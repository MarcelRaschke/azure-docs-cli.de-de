---
title: Verwenden von Azure-Dienstprinzipalen mit der Azure CLI 2.0
description: Hier erfahren Sie, wie Sie mit der Azure CLI 2.0 einen Dienstprinzipal erstellen und verwenden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: role-based-access-control
ms.openlocfilehash: cd9a41b66d18410afa091ede50ca24e7d4b5e9ed
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439957"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0

Wenn Sie eine separate Anmeldung mit Zugriffseinschränkungen erstellen möchten, können Sie dafür einen Dienstprinzipal verwenden. Dienstprinzipale sind separate Identitäten, die einem Konto zugeordnet werden können. Dienstprinzipale sind hilfreich bei der Verwendung von Anwendungen und Tasks, die automatisiert werden müssen. Dieser Artikel führt Sie durch den Vorgang zum Erstellen eines Dienstprinzipals.

## <a name="create-the-service-principal"></a>Erstellen des Dienstprinzipals

Verwenden Sie den Befehl [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac), um einen Dienstprinzipal zu erstellen. Der Name des Dienstprinzipals ist nicht mit dem vorhandenen Namen einer Anwendung oder eines Benutzers verknüpft. Sie können einen Dienstprinzipal mit dem gewünschten Authentifizierungstyp erstellen.

* `--password` wird für die kennwortbasierte Authentifizierung verwendet. Halten Sie sich an die Vorgaben unter [Kennwortrichtlinien und -einschränkungen in Azure Active Directory](/azure/active-directory/active-directory-passwords-policy), um ein sicheres Kennwort zu erstellen. Falls Sie kein Kennwort angeben, wird eines für Sie erstellt.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* `--cert` wird für die zertifikatbasierte Authentifizierung für ein vorhandenes Zertifikat verwendet (entweder als öffentliche PEM- oder DER-Zeichenfolge oder als `@{file}` zum Laden einer Datei).

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  Das Argument `--keyvault` kann hinzugefügt werden, um anzugeben, dass das Zertifikat in Azure Key Vault gespeichert wird. In diesem Fall verweist der Wert `--cert` auf den Namen des Zertifikats in Key Vault.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* `--create-cert` erstellt ein _selbstsigniertes_ Zertifikat für die Authentifizierung. Wenn das Argument `--cert` nicht angegeben wird, wird ein zufälliger Zertifikatname generiert.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  Das Argument `--keyvault` kann hinzugefügt werden, um das Zertifikat in Azure Key Vault zu speichern. Bei Verwendung von `--keyvault` ist auch das Argument `--cert` erforderlich.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

Wenn kein Argument angegeben wird, das den Authentifizierungstyp angibt, wird standardmäßig `--password` verwendet.

Die Ausgabe des Befehls `create-for-rbac` hat folgendes Format:

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Die Werte `appId`, `tenant` und `password` werden für die Authentifizierung verwendet. `displayName` wird bei der Suche nach einem vorhandenen Dienstprinzipal verwendet.

> [!NOTE]
> Wenn Ihr Konto nicht über ausreichende Berechtigungen zum Erstellen eines Dienstprinzipals verfügt, wird eine Fehlermeldung mit dem Hinweis „Nicht genügend Berechtigungen zum Abschließen des Vorgangs“ angezeigt. Bitten Sie den Azure Active Directory-Administrator, einen Dienstprinzipal zu erstellen.

## <a name="manage-service-principal-roles"></a>Verwalten von Dienstprinzipalrollen 

Die Azure CLI 2.0 enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**. Diese Rolle besitzt uneingeschränkte Berechtigungen für Lese- und Schreibvorgänge in einem Azure-Konto. Sie eignet sich in der Regel nicht für Anwendungen. Die Rolle **Leser** ist stärker eingeschränkt und bietet schreibgeschützten Zugriff.  Weitere Informationen zur rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) und zu Rollen finden Sie unter [Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).

Dieses Beispiel fügt die Rolle **Leser** hinzu und löscht die Rolle **Mitwirkender**.

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

Durch das Hinzufügen einer Rolle werden zuvor zugewiesene Berechtigungen _nicht_ geändert. Beim Einschränken der Berechtigungen eines Dienstprinzipals sollte immer die Rolle __Mitwirkender__ entfernt werden.

Die Änderungen können durch Auflisten der zugewiesenen Rollen überprüft werden.

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> Wenn Ihr Konto nicht über die Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ über Bereich „/subscriptions/{guid}“ hat. Bitten Sie den Azure Active Directory-Administrator um die Verwaltung von Rollen.

## <a name="sign-in-using-the-service-principal"></a>Anmelden mithilfe des Dienstprinzipals

Sie können die Anmeldung und Berechtigungen des neuen Dienstprinzipals testen, indem Sie sich darunter bei der Azure CLI anmelden. Melden Sie sich mit den Werten für `appId`, `tenant` und die Anmeldeinformationen an. Die von Ihnen angegebenen Authentifizierungsinformationen ändern sich basierend darauf, ob Sie den Dienstprinzipal mit einem Kennwort oder mit einem Zertifikat erstellen möchten.

Wenn Sie sich mit einem Kennwort anmelden möchten, geben Sie es als Argumentparameter an.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Um sich mit einem Zertifikat anmelden zu können, muss es lokal als PEM- oder DER-Datei verfügbar sein.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>Zurücksetzen von Anmeldeinformation

Falls Sie die Anmeldeinformationen für einen Dienstprinzipal vergessen, können sie mit dem Befehl [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) zurückgesetzt werden. Hier gelten die gleichen Einschränkungen und Optionen wie beim Erstellen eines neuen Dienstprinzipals.

```azurecli-interactive
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```

---
title: Anmelden mit der Azure CLI
description: Melden Sie sich interaktiv mit der Azure CLI oder mit lokalen Anmeldeinformationen an.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/22/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 97873602f04c02bf69cd1465b84f99633a8cbd9f
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581528"
---
# <a name="sign-in-with-azure-cli"></a>Anmelden mit der Azure CLI 

Es gibt mehrere Authentifizierungstypen für die Azure CLI. Den einfachsten Einstieg ermöglicht der [Azure Cloud Shell](/azure/cloud-shell/overview)-Dienst, der Sie automatisch anmeldet.
Lokal können Sie sich interaktiv über Ihren Browser mit dem Befehl [az login](/cli/azure/reference-index#az_login) anmelden. Beim Schreiben von Skripts wird die Verwendung von Dienstprinzipalen empfohlen. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierung schützen.

Ihre Anmeldeinformationen werden nicht von der CLI gespeichert. Stattdessen wird von Azure ein [Authentifizierungsaktualisierungstoken](/azure/active-directory/develop/v1-id-and-access-tokens#refresh-tokens) generiert und gespeichert. Ab August 2018 wird dieses Token nach 90-tägiger Inaktivität widerrufen. Dieser Wert kann jedoch von Microsoft oder von Ihrem Mandantenadministrator geändert werden. Wenn das Token widerrufen wurde, werden Sie von der Befehlszeilenschnittstelle aufgefordert, sich erneut anzumelden.

Nach der Anmeldung werden CLI-Befehle für Ihr Standardabonnement ausgeführt. Sollten Sie über mehrere Abonnements verfügen, können Sie das [Standardabonnement ändern](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Interaktives Anmelden

Die Standardauthentifizierungsmethode der Azure CLI ist die Anmeldung über einen Webbrowser mit Zugriffstoken.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Anmelden mit Anmeldeinformationen über die Befehlszeile

Geben Sie Ihre Azure-Benutzeranmeldeinformationen in der Befehlszeile an.

> [!Note]
> Dieser Ansatz funktioniert nicht für Microsoft-Konten oder Konten, für die die Authentifizierung in zwei Schritten aktiviert ist.

```azurecli-interactive
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Wenn Sie die Anzeige Ihres Kennworts in der Konsole vermeiden möchten und `az login` interaktiv verwenden, können Sie den Befehl `read -s` unter `bash` nutzen.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> Verwenden Sie in PowerShell das Cmdlet `Get-Credential`.
>
> ```powershell
> $AzCred = Get-Credential -UserName <username>
> az login -u $AzCred.UserName -p $AzCred.GetNetworkCredential().Password
> ```

## <a name="sign-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind Konten, die nicht an einen bestimmten Benutzer gebunden sind und über Berechtigungen verfügen können, die ihnen über vordefinierte Rollen zugewiesen werden. Die Authentifizierung mit einem Dienstprinzipal ist die beste Methode zum Schreiben sicherer Skripts oder Programme und ermöglicht das Anwenden von Berechtigungseinschränkungen und lokal gespeicherten statischen Anmeldeinformationen. Weitere Informationen zu Dienstprinzipalen finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0](./create-an-azure-service-principal-azure-cli.md#sign-in-using-a-service-principal).

Für die Anmeldung mit einem Dienstprinzipal benötigen Sie Folgendes:

* Die dem Dienstprinzipal zugeordnete URL bzw. den zugeordneten Namen
* Das Dienstprinzipalkennwort oder das X509-Zertifikat (im PEM-Format), das zum Erstellen des Dienstprinzipals verwendet wurde
* Den dem Dienstprinzipal zugeordneten Mandanten, als `.onmicrosoft.com`-Domäne oder Azure-Objekt-ID

> [!NOTE]
> In einer PEM-Datei muss ein Zertifikat (**CERTIFICATE**) an den privaten Schlüssel (**PRIVATE KEY**) angefügt werden.  Ein Beispiel für ein PEM-Dateiformat finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit der Azure-Befehlszeilenschnittstelle](./create-an-azure-service-principal-azure-cli.md#sign-in-using-a-service-principal). 
>

> [!IMPORTANT]
>
> Falls Ihr Dienstprinzipal ein in Key Vault gespeichertes Zertifikat nutzt, muss der private Schlüssel des Zertifikats verfügbar sein, ohne dass eine Anmeldung bei Azure erforderlich ist. Verwenden Sie [az keyvault secret show](/cli/azure/keyvault/secret), um einen privaten Schlüssel zur Offlineverwendung abzurufen.

```azurecli-interactive
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

> [!IMPORTANT]
> Wenn Sie die Anzeige Ihres Kennworts in der Konsole vermeiden möchten und `az login` interaktiv verwenden, können Sie den Befehl `read -s` unter `bash` nutzen.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> Verwenden Sie in PowerShell das Cmdlet `Get-Credential`.
>
> ```powershell
> $AzCred = Get-Credential -UserName <app-url>
> az login --service-principal -u $AzCred.UserName -p $AzCred.GetNetworkCredential().Password --tenant <tenant>
> ```

## <a name="sign-in-with-a-different-tenant"></a>Anmelden mit einem anderen Mandanten

Sie können mit dem Argument `--tenant` einen Mandanten auswählen, unter dem Sie sich anmelden möchten. Der Wert dieses Arguments kann eine Domäne vom Typ `.onmicrosoft.com` oder die Azure-Objekt-ID für den Mandanten sein. Mit `--tenant` können sowohl interaktive Methoden als auch die Befehlszeile für die Anmeldung verwendet werden.

```azurecli-interactive
az login --tenant <tenant>
```

## <a name="sign-in-with-a-managed-identity"></a>Anmelden mit einer verwalteten Identität

Auf Ressourcen, die für verwaltete Identitäten von Azure-Ressourcen konfiguriert sind, können Sie sich mit der verwalteten Identität anmelden. Das Anmelden mit der Identität der Ressource erfolgt über das Flag `--identity`.

```azurecli-interactive
az login --identity
```

Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Konfigurieren von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer mithilfe der Azure-Befehlszeilenschnittstelle](/azure/active-directory/managed-identities-azure-resources/qs-configure-cli-windows-vm) und [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer für die Anmeldung](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-sign-in).
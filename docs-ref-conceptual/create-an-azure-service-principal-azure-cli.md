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
ms.openlocfilehash: d250cb2d35a128c789fccd3aca17c47074121a25
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703110"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="c84f9-103">Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c84f9-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="c84f9-104">Wenn Sie eine separate Anmeldung mit Zugriffseinschränkungen erstellen möchten, können Sie dafür einen Dienstprinzipal verwenden.</span><span class="sxs-lookup"><span data-stu-id="c84f9-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="c84f9-105">Dienstprinzipale sind separate Identitäten, die einem Konto zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="c84f9-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="c84f9-106">Dienstprinzipale sind hilfreich bei der Verwendung von Anwendungen und Tasks, die automatisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="c84f9-107">Dieser Artikel führt Sie durch den Vorgang zum Erstellen eines Dienstprinzipals.</span><span class="sxs-lookup"><span data-stu-id="c84f9-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="c84f9-108">Erstellen des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="c84f9-108">Create the service principal</span></span>

<span data-ttu-id="c84f9-109">Verwenden Sie den Befehl [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac), um einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="c84f9-110">Der Name des Dienstprinzipals ist nicht mit dem vorhandenen Namen einer Anwendung oder eines Benutzers verknüpft.</span><span class="sxs-lookup"><span data-stu-id="c84f9-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="c84f9-111">Sie können einen Dienstprinzipal mit dem gewünschten Authentifizierungstyp erstellen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="c84f9-112">`--password` wird für die kennwortbasierte Authentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="c84f9-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="c84f9-113">Halten Sie sich an die Vorgaben unter [Kennwortrichtlinien und -einschränkungen in Azure Active Directory](/azure/active-directory/active-directory-passwords-policy), um ein sicheres Kennwort zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="c84f9-114">Falls Sie kein Kennwort angeben, wird eines für Sie erstellt.</span><span class="sxs-lookup"><span data-stu-id="c84f9-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="c84f9-115">`--cert` wird für die zertifikatbasierte Authentifizierung für ein vorhandenes Zertifikat verwendet (entweder als öffentliche PEM- oder DER-Zeichenfolge oder als `@{file}` zum Laden einer Datei).</span><span class="sxs-lookup"><span data-stu-id="c84f9-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="c84f9-116">Das Argument `--keyvault` kann hinzugefügt werden, um anzugeben, dass das Zertifikat in Azure Key Vault gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="c84f9-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="c84f9-117">In diesem Fall verweist der Wert `--cert` auf den Namen des Zertifikats in Key Vault.</span><span class="sxs-lookup"><span data-stu-id="c84f9-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="c84f9-118">`--create-cert` erstellt ein _selbstsigniertes_ Zertifikat für die Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="c84f9-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="c84f9-119">Wenn das Argument `--cert` nicht angegeben wird, wird ein zufälliger Zertifikatname generiert.</span><span class="sxs-lookup"><span data-stu-id="c84f9-119">If the `--cert` argument is not provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="c84f9-120">Das Argument `--keyvault` kann hinzugefügt werden, um das Zertifikat in Azure Key Vault zu speichern.</span><span class="sxs-lookup"><span data-stu-id="c84f9-120">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="c84f9-121">Bei Verwendung von `--keyvault` ist auch das Argument `--cert` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c84f9-121">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="c84f9-122">Wenn kein Argument angegeben wird, das den Authentifizierungstyp angibt, wird standardmäßig `--password` verwendet.</span><span class="sxs-lookup"><span data-stu-id="c84f9-122">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="c84f9-123">Die Ausgabe des Befehls `create-for-rbac` hat folgendes Format:</span><span class="sxs-lookup"><span data-stu-id="c84f9-123">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="c84f9-124">Die Werte `appId`, `tenant` und `password` werden für die Authentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="c84f9-124">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="c84f9-125">`displayName` wird bei der Suche nach einem vorhandenen Dienstprinzipal verwendet.</span><span class="sxs-lookup"><span data-stu-id="c84f9-125">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="c84f9-126">Wenn Ihr Konto nicht über ausreichende Berechtigungen zum Erstellen eines Dienstprinzipals verfügt, wird eine Fehlermeldung mit dem Hinweis „Nicht genügend Berechtigungen zum Abschließen des Vorgangs“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c84f9-126">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="c84f9-127">Bitten Sie den Azure Active Directory-Administrator, einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-127">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="c84f9-128">Verwalten von Dienstprinzipalrollen</span><span class="sxs-lookup"><span data-stu-id="c84f9-128">Manage service principal roles</span></span> 

<span data-ttu-id="c84f9-129">Die Azure CLI 2.0 enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:</span><span class="sxs-lookup"><span data-stu-id="c84f9-129">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="c84f9-130">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="c84f9-130">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="c84f9-131">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="c84f9-131">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="c84f9-132">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="c84f9-132">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="c84f9-133">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="c84f9-133">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="c84f9-134">Diese Rolle besitzt uneingeschränkte Berechtigungen für Lese- und Schreibvorgänge in einem Azure-Konto. Sie eignet sich in der Regel nicht für Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-134">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="c84f9-135">Die Rolle **Leser** ist stärker eingeschränkt und bietet schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="c84f9-135">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="c84f9-136">Weitere Informationen zur rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) und zu Rollen finden Sie unter [Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="c84f9-136">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="c84f9-137">Dieses Beispiel fügt die Rolle **Leser** hinzu und löscht die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="c84f9-137">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="c84f9-138">Durch das Hinzufügen einer Rolle werden zuvor zugewiesene Berechtigungen _nicht_ geändert.</span><span class="sxs-lookup"><span data-stu-id="c84f9-138">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="c84f9-139">Beim Einschränken der Berechtigungen eines Dienstprinzipals sollte immer die Rolle __Mitwirkender__ entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="c84f9-139">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="c84f9-140">Die Änderungen können durch Auflisten der zugewiesenen Rollen überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="c84f9-140">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="c84f9-141">Wenn Ihr Konto nicht über die Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ über Bereich „/subscriptions/{guid}“ hat. Bitten Sie den Azure Active Directory-Administrator um die Verwaltung von Rollen.</span><span class="sxs-lookup"><span data-stu-id="c84f9-141">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="log-in-using-the-service-principal"></a><span data-ttu-id="c84f9-142">Anmelden mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="c84f9-142">Log in using the service principal</span></span>

<span data-ttu-id="c84f9-143">Sie können die Anmeldung und Berechtigungen des neuen Dienstprinzipals testen, indem Sie sich darunter bei der Azure CLI anmelden.</span><span class="sxs-lookup"><span data-stu-id="c84f9-143">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="c84f9-144">Melden Sie sich mit den Werten für `appId`, `tenant` und die Anmeldeinformationen an.</span><span class="sxs-lookup"><span data-stu-id="c84f9-144">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="c84f9-145">Die von Ihnen angegebenen Authentifizierungsinformationen ändern sich basierend darauf, ob Sie den Dienstprinzipal mit einem Kennwort oder mit einem Zertifikat erstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="c84f9-145">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="c84f9-146">Wenn Sie sich mit einem Kennwort anmelden möchten, geben Sie es als Argumentparameter an.</span><span class="sxs-lookup"><span data-stu-id="c84f9-146">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="c84f9-147">Um sich mit einem Zertifikat anmelden zu können, muss es lokal als PEM- oder DER-Datei verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="c84f9-147">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="c84f9-148">Zurücksetzen von Anmeldeinformation</span><span class="sxs-lookup"><span data-stu-id="c84f9-148">Reset credentials</span></span>

<span data-ttu-id="c84f9-149">Falls Sie die Anmeldeinformationen für einen Dienstprinzipal vergessen, können sie mit dem Befehl [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) zurückgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="c84f9-149">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) command.</span></span> <span data-ttu-id="c84f9-150">Hier gelten die gleichen Einschränkungen und Optionen wie beim Erstellen eines neuen Dienstprinzipals.</span><span class="sxs-lookup"><span data-stu-id="c84f9-150">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```

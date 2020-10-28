---
title: Verwenden von Azure-Dienstprinzipalen mit der Azure CLI
description: Hier erfahren Sie, wie Sie mit der Azure-Befehlszeilenschnittstelle Dienstprinzipale erstellen und verwenden.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/15/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 17f550e2ce1df2e171d51c262d7a5e0428965039
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "92686998"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a><span data-ttu-id="d40f4-103">Erstellen eines Azure-Dienstprinzipals mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="d40f4-103">Create an Azure service principal with the Azure CLI</span></span>

<span data-ttu-id="d40f4-104">Für automatisierte Tools, die Azure-Dienste verwenden, sollten stets eingeschränkte Berechtigungen festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="d40f4-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="d40f4-105">Azure bietet Dienstprinzipale, damit Anwendungen nicht als Benutzer mit uneingeschränkten Berechtigungen angemeldet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="d40f4-106">Ein Azure-Dienstprinzipal ist eine Identität, die zur Verwendung mit Anwendungen, gehosteten Diensten und automatisierten Tools für den Zugriff auf Azure-Ressourcen erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d40f4-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="d40f4-107">Dieser Zugriff wird durch die dem Dienstprinzipal zugewiesenen Rollen eingeschränkt. Dadurch können Sie steuern, auf welcher Ebene auf welche Ressourcen zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="d40f4-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="d40f4-108">Aus Sicherheitsgründen wird stets empfohlen, Dienstprinzipale mit automatisierten Tools zu verwenden, statt ihnen die Anmeldung mit einer Benutzeridentität zu erlauben.</span><span class="sxs-lookup"><span data-stu-id="d40f4-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="d40f4-109">In diesem Artikel wird Schritt für Schritt erläutert, wie Sie mit der Azure CLI einen Dienstprinzipal erstellen, Informationen zu ihm abrufen und ihn zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="d40f4-110">Erstellen eines Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="d40f4-110">Create a service principal</span></span>

<span data-ttu-id="d40f4-111">Erstellen Sie mit dem Befehl [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) einen Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="d40f4-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="d40f4-112">Beim Erstellen eines Dienstprinzipals wählen Sie den Typ der von ihm verwendeten Anmeldeauthentifizierung aus.</span><span class="sxs-lookup"><span data-stu-id="d40f4-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="d40f4-113">Wenn Ihr Konto nicht über Berechtigungen zum Erstellen eines Dienstprinzipals verfügt, gibt `az ad sp create-for-rbac` eine Fehlermeldung mit dem Hinweis „Nicht genügend Berechtigungen zum Abschließen des Vorgangs“ zurück.</span><span class="sxs-lookup"><span data-stu-id="d40f4-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="d40f4-114">Bitten Sie den Azure Active Directory-Administrator, einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="d40f4-115">Für Dienstprinzipale stehen zwei Authentifizierungstypen zur Verfügung: Kennwortbasierte Authentifizierung und zertifikatbasierte Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="d40f4-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="d40f4-116">Kennwortbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="d40f4-116">Password-based authentication</span></span>

<span data-ttu-id="d40f4-117">Ohne jegliche Authentifizierungsparameter wird die kennwortbasierte Authentifizierung mit einem für Sie erstellten zufälligen Kennwort verwendet.</span><span class="sxs-lookup"><span data-stu-id="d40f4-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="d40f4-118">Ab Azure CLI 2.0.68 wird der Parameter `--password` zum Erstellen eines Dienstprinzipals mit einem benutzerdefinierten Kennwort __nicht mehr unterstützt__ , um die versehentliche Verwendung von unsicheren Kennwörtern zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="d40f4-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="d40f4-119">Die Ausgabe für einen Dienstprinzipal mit Kennwortauthentifizierung enthält den Schlüssel `password`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="d40f4-120">Kopieren Sie diesen Wert __unbedingt__ , da er nicht abgerufen werden kann.</span><span class="sxs-lookup"><span data-stu-id="d40f4-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="d40f4-121">Wenn Sie das Kennwort vergessen haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d40f4-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="d40f4-122">Die Schlüssel `appId` und `tenant` werden in der Ausgabe von `az ad sp create-for-rbac` angezeigt und bei der Dienstprinzipalauthentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="d40f4-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="d40f4-123">Notieren Sie die Werte. Sie können jedoch auch jederzeit mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="d40f4-124">Zertifikatbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="d40f4-124">Certificate-based authentication</span></span>

<span data-ttu-id="d40f4-125">Verwenden Sie für die zertifikatbasierte Authentifizierung das Argument `--cert`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="d40f4-126">Bei Verwendung dieses Arguments muss bereits ein Zertifikat vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="d40f4-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="d40f4-127">Vergewissern Sie sich, dass alle Tools, die diesen Dienstprinzipal verwenden, Zugriff auf den privaten Schlüssel des Zertifikats haben.</span><span class="sxs-lookup"><span data-stu-id="d40f4-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="d40f4-128">Zertifikate müssen in einem ASCII-Format vorliegen, etwa PEM, CER oder DER.</span><span class="sxs-lookup"><span data-stu-id="d40f4-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="d40f4-129">Übergeben Sie das Zertifikat als Zeichenfolge, oder verwenden Sie das Format `@path`, um das Zertifikat aus einer Datei zu laden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

> [!NOTE]
> <span data-ttu-id="d40f4-130">Bei Verwendung einer PEM-Datei muss das Zertifikat ( **CERTIFICATE** ) an den privaten Schlüssel ( **PRIVATE KEY** ) in der Datei angefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-130">When using a PEM file, the **CERTIFICATE** must be appended to the **PRIVATE KEY** within the file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="d40f4-131">Das Argument `--keyvault` kann hinzugefügt werden, um ein Zertifikat in Azure Key Vault zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-131">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="d40f4-132">In diesem Fall ist der Wert `--cert` der Name des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="d40f4-132">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="d40f4-133">Verwenden Sie das Argument `--create-cert`, um ein _selbstsigniertes_ Zertifikat für die Authentifizierung zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="d40f4-133">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="d40f4-134">Konsolenausgabe:</span><span class="sxs-lookup"><span data-stu-id="d40f4-134">Console output:</span></span>

```
Creating a role assignment under the scope of "/subscriptions/myId"
Please copy C:\myPath\myNewFile.pem to a safe place.
When you run 'az login', provide the file path in the --password argument
{
  "appId": "myAppId",
  "displayName": "myDisplayName",
  "fileWithCertAndPrivateKey": "C:\\myPath\\myNewFile.pem",
  "name": "http://myName",
  "password": null,
  "tenant": "myTenantId"
}
```

<span data-ttu-id="d40f4-135">Inhalt der neuen PEM-Datei:</span><span class="sxs-lookup"><span data-stu-id="d40f4-135">Contents of the new PEM file:</span></span>
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> <span data-ttu-id="d40f4-136">Mit dem Befehl `az ad sp create-for-rbac --create-cert` werden der Dienstprinzipal und eine PEM-Datei erstellt.</span><span class="sxs-lookup"><span data-stu-id="d40f4-136">The `az ad sp create-for-rbac --create-cert` command creates the service principal and a PEM file.</span></span> <span data-ttu-id="d40f4-137">Die PEM-Datei enthält einen ordnungsgemäß formatierten privaten Schlüssel ( **PRIVATE KEY** ) und ein ordnungsgemäß formatiertes Zertifikat ( **CERTIFICATE** ).</span><span class="sxs-lookup"><span data-stu-id="d40f4-137">The PEM file contains a correctly formatted **PRIVATE KEY** and **CERTIFICATE** .</span></span>

<span data-ttu-id="d40f4-138">Das Argument `--keyvault` kann hinzugefügt werden, um das Zertifikat in Azure Key Vault zu speichern.</span><span class="sxs-lookup"><span data-stu-id="d40f4-138">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="d40f4-139">Bei Verwendung von `--keyvault` ist das Argument `--cert`__erforderlich__ .</span><span class="sxs-lookup"><span data-stu-id="d40f4-139">When using `--keyvault`, the `--cert` argument is __required__ .</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="d40f4-140">Die Ausgabe enthält den Schlüssel `fileWithCertAndPrivateKey`, es sei denn, Sie speichern das Zertifikat in Key Vault.</span><span class="sxs-lookup"><span data-stu-id="d40f4-140">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="d40f4-141">Am Wert dieses Schlüssels können Sie erkennen, wo das generierte Zertifikat gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="d40f4-141">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="d40f4-142">Kopieren Sie das Zertifikat __unbedingt__ an einen sicheren Speicherort. Andernfalls können Sie sich nicht mit diesem Dienstprinzipal anmelden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-142">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="d40f4-143">Rufen Sie für in Key Vault gespeicherte Zertifikate den privaten Schlüssel des Zertifikats mit [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show) ab.</span><span class="sxs-lookup"><span data-stu-id="d40f4-143">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="d40f4-144">In Key Vault ist der Name des Zertifikatgeheimnisses mit dem Zertifikatnamen identisch.</span><span class="sxs-lookup"><span data-stu-id="d40f4-144">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="d40f4-145">Wenn Sie keinen Zugriff mehr auf den privaten Schlüssel des Zertifikats haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d40f4-145">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="d40f4-146">Die Schlüssel `appId` und `tenant` werden in der Ausgabe von `az ad sp create-for-rbac` angezeigt und bei der Dienstprinzipalauthentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="d40f4-146">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="d40f4-147">Notieren Sie die Werte. Sie können jedoch auch jederzeit mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-147">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="d40f4-148">Abrufen eines vorhandenen Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="d40f4-148">Get an existing service principal</span></span>

<span data-ttu-id="d40f4-149">Mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) kann eine Liste der Dienstprinzipale in einem Mandanten abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-149">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="d40f4-150">Dieser Befehl gibt standardmäßig die ersten 100 Dienstprinzipale für Ihren Mandanten zurück.</span><span class="sxs-lookup"><span data-stu-id="d40f4-150">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="d40f4-151">Verwenden Sie zum Abrufen aller Dienstprinzipale eines Mandanten das Argument `--all`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-151">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="d40f4-152">Da das Abrufen dieser Liste sehr lange dauern kann, wird empfohlen, die Liste mit einem der folgenden Argumente zu filtern:</span><span class="sxs-lookup"><span data-stu-id="d40f4-152">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="d40f4-153">`--display-name` fordert Dienstprinzipale mit einem _Präfix_ an, das dem angegebenen Namen entspricht.</span><span class="sxs-lookup"><span data-stu-id="d40f4-153">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="d40f4-154">Der Anzeigename eines Dienstprinzipals ist der Wert, der während der Erstellung mit dem Parameter `--name` festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="d40f4-154">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="d40f4-155">Haben Sie `--name` während der Erstellung des Dienstprinzipals nicht festgelegt, lautet das Namenspräfix `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-155">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="d40f4-156">`--spn` filtert nach genauen Übereinstimmungen des Dienstprinzipalnamens.</span><span class="sxs-lookup"><span data-stu-id="d40f4-156">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="d40f4-157">Der Dienstprinzipalname beginnt immer mit `https://`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-157">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="d40f4-158">Handelte es sich bei dem für `--name` verwendeten Wert nicht um einen URI, wird für diesen Wert `https://` gefolgt vom Anzeigenamen verwendet.</span><span class="sxs-lookup"><span data-stu-id="d40f4-158">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="d40f4-159">`--show-mine` fordert nur Dienstprinzipale an, die vom angemeldeten Benutzer erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-159">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="d40f4-160">`--filter` akzeptiert einen OData-Filter und führt die _serverseitige_ Filterung aus.</span><span class="sxs-lookup"><span data-stu-id="d40f4-160">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="d40f4-161">Diese Methode wird anstelle der clientseitigen Filterung mit dem Argument `--query` der CLI empfohlen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-161">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="d40f4-162">Weitere Informationen zu OData-Filtern finden Sie unter [OData-Ausdruckssyntax für Filter und Sortierklauseln in Azure Search](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="d40f4-162">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="d40f4-163">Für Dienstprinzipalobjekte werden ausführliche Informationen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d40f4-163">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="d40f4-164">Verwenden Sie die Abfragezeichenfolge `[].{id:appId, tenant:appOwnerTenantId}`, um nur die für die Anmeldung erforderlichen Informationen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-164">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="d40f4-165">Die Anmeldeinformationen für alle Dienstprinzipale, die vom derzeit angemeldeten Benutzer erstellt wurden, rufen Sie beispielsweise wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="d40f4-165">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="d40f4-166">Mit `az ad sp list` und [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) rufen Sie den Benutzer und den Mandanten ab, allerdings nicht die Authentifizierungsgeheimnisse _oder_ die Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="d40f4-166">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="d40f4-167">Geheimnisse für Zertifikate in Key Vault können mit [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show) abgerufen werden. Andere Geheimnisse werden jedoch nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d40f4-167">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="d40f4-168">Wenn Sie eine Authentifizierungsmethode oder ein Geheimnis vergessen haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d40f4-168">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="d40f4-169">Verwalten von Dienstprinzipalrollen</span><span class="sxs-lookup"><span data-stu-id="d40f4-169">Manage service principal roles</span></span>

<span data-ttu-id="d40f4-170">Die Azure CLI enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:</span><span class="sxs-lookup"><span data-stu-id="d40f4-170">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="d40f4-171">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="d40f4-171">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="d40f4-172">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="d40f4-172">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="d40f4-173">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="d40f4-173">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="d40f4-174">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender** .</span><span class="sxs-lookup"><span data-stu-id="d40f4-174">The default role for a service principal is **Contributor** .</span></span> <span data-ttu-id="d40f4-175">Diese Rolle besitzt uneingeschränkte Berechtigungen für Lese- und Schreibvorgänge in einem Azure-Konto.</span><span class="sxs-lookup"><span data-stu-id="d40f4-175">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="d40f4-176">Die Rolle **Leser** ist stärker eingeschränkt und bietet schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="d40f4-176">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="d40f4-177">Weitere Informationen zur rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) finden Sie unter [Rollenbasierte Zugriffssteuerung: Integrierte Rollen](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="d40f4-177">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="d40f4-178">Das folgende Beispiel fügt die Rolle **Leser** hinzu und entfernt die Rolle **Mitwirkender** :</span><span class="sxs-lookup"><span data-stu-id="d40f4-178">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="d40f4-179">Wenn Ihr Konto nicht über Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ hat. Bitten Sie den Azure Active Directory-Administrator um die Verwaltung von Rollen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-179">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="d40f4-180">Durch das Hinzufügen einer Rolle werden zuvor zugewiesene Berechtigungen _nicht_ eingeschränkt.</span><span class="sxs-lookup"><span data-stu-id="d40f4-180">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="d40f4-181">Beim Einschränken der Berechtigungen eines Dienstprinzipals sollte die Rolle __Mitwirkender__ entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-181">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="d40f4-182">Die Änderungen können durch Auflisten der zugewiesenen Rollen überprüft werden:</span><span class="sxs-lookup"><span data-stu-id="d40f4-182">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="d40f4-183">Anmelden mithilfe eines Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="d40f4-183">Sign in using a service principal</span></span>

<span data-ttu-id="d40f4-184">Testen Sie die Anmeldeinformationen und Berechtigungen des neuen Dienstprinzipals, indem Sie sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-184">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="d40f4-185">Für die Anmeldung mit einem Dienstprinzipal benötigen Sie `appId`, `tenant` und Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="d40f4-185">To sign in with a service principal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="d40f4-186">So melden Sie sich mit einem Dienstprinzipal und einem Kennwort an:</span><span class="sxs-lookup"><span data-stu-id="d40f4-186">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="d40f4-187">Um sich mit einem Zertifikat anmelden zu können, muss es lokal als PEM- oder DER-Datei im ASCII-Format verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="d40f4-187">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format.</span></span> <span data-ttu-id="d40f4-188">Bei Verwendung einer PEM-Datei müssen der private Schlüssel ( **PRIVATE KEY** ) und das Zertifikat ( **CERTIFICATE** ) gemeinsam innerhalb der Datei angefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-188">When using a PEM file, the **PRIVATE KEY** and **CERTIFICATE** must be appended together within the file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="d40f4-189">Weitere Informationen zum Anmelden mit einem Dienstprinzipal finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d40f4-189">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="create-a-resource-using-service-principal"></a><span data-ttu-id="d40f4-190">Erstellen einer Ressource mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="d40f4-190">Create a resource using service principal</span></span>

<span data-ttu-id="d40f4-191">Der folgende Abschnitt enthält ein Beispiel für die Erstellung einer Ressource für [Azure Storage](/azure/storage/) mit einem Dienstprinzipal. Dazu werden die folgenden Befehle verwendet:</span><span class="sxs-lookup"><span data-stu-id="d40f4-191">The following section provides an example of how to create an resource for [Azure Storage](/azure/storage/) with a service principal, using the following commands:</span></span>

* [<span data-ttu-id="d40f4-192">az login</span><span class="sxs-lookup"><span data-stu-id="d40f4-192">az login</span></span>](/cli/azure/reference-index?#az_login)
* [<span data-ttu-id="d40f4-193">az group create</span><span class="sxs-lookup"><span data-stu-id="d40f4-193">az group create</span></span>](/cli/azure/group#az_group_create)
* [<span data-ttu-id="d40f4-194">az storage account create</span><span class="sxs-lookup"><span data-stu-id="d40f4-194">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)
* [<span data-ttu-id="d40f4-195">az storage account keys list</span><span class="sxs-lookup"><span data-stu-id="d40f4-195">az storage account keys list</span></span>](/cli/azure/storage/account/keys#az_storage_account_keys_list)

<span data-ttu-id="d40f4-196">Für die Anmeldung mit einem Dienstprinzipal benötigen Sie die Werte für `appId`, `tenant` und `password`, die beim [Erstellen des Dienstprinzipals](#sign-in-using-a-service-principal) als Antwort zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-196">To sign in with a service principal, you need the `appId`, `tenant`, and `password` returned as the response when you [created your service principal](#sign-in-using-a-service-principal).</span></span>

1. <span data-ttu-id="d40f4-197">Melden Sie sich als Dienstprinzipal an.</span><span class="sxs-lookup"><span data-stu-id="d40f4-197">Log in as the service principal.</span></span>

    ```azurecli-interactive
    az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
    ```

1. <span data-ttu-id="d40f4-198">Erstellen Sie eine Ressourcengruppe für alle Ressourcen, die für den gleichen Schnellstart, das gleiche Tutorial oder das gleiche Entwicklungsprojekt verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d40f4-198">Create a resource group to hold all resources used for the same quickstart, tutorial, or development project.</span></span>

    ```azurecli-interactive
    az group create --location WESTUS --name MY_RESOURCE_GROUP
    ```

1. <span data-ttu-id="d40f4-199">Erstellen Sie eine Ressource für einen Azure-Dienst.</span><span class="sxs-lookup"><span data-stu-id="d40f4-199">Create a resource to an Azure service.</span></span> <span data-ttu-id="d40f4-200">Ersetzen Sie `<SERVICENAME>` durch den Namen des Azure-Diensts.</span><span class="sxs-lookup"><span data-stu-id="d40f4-200">Replace `<SERVICENAME>` with the name of the Azure service.</span></span>

    <span data-ttu-id="d40f4-201">Für Azure Storage sind folgende Werte für den Parameter `<KIND>` zulässig:</span><span class="sxs-lookup"><span data-stu-id="d40f4-201">For Azure Storage, valid values for the `<KIND>` parameter are:</span></span>

    * <span data-ttu-id="d40f4-202">BlobStorage</span><span class="sxs-lookup"><span data-stu-id="d40f4-202">BlobStorage</span></span>
    * <span data-ttu-id="d40f4-203">BlockBlobStorage</span><span class="sxs-lookup"><span data-stu-id="d40f4-203">BlockBlobStorage</span></span>
    * <span data-ttu-id="d40f4-204">FileStorage</span><span class="sxs-lookup"><span data-stu-id="d40f4-204">FileStorage</span></span>
    * <span data-ttu-id="d40f4-205">Storage</span><span class="sxs-lookup"><span data-stu-id="d40f4-205">Storage</span></span>
    * <span data-ttu-id="d40f4-206">StorageV2</span><span class="sxs-lookup"><span data-stu-id="d40f4-206">StorageV2</span></span>

    ```azurecli-interactive
    az storage account create --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP --kind <KIND> --sku F0 --location WESTUS --yes
    ```

1. <span data-ttu-id="d40f4-207">Rufen Sie Ressourcenschlüssel für die neue Ressource ab. Sie verwenden ihn in Ihrem Code zum Authentifizieren beim Azure-Dienst.</span><span class="sxs-lookup"><span data-stu-id="d40f4-207">Get resource keys for the new resource, which you use in your code to authenticate to the Azure service.</span></span>

    ```azurecli-interactive
    az storage account keys list --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP
    ```

## <a name="reset-credentials"></a><span data-ttu-id="d40f4-208">Zurücksetzen von Anmeldeinformation</span><span class="sxs-lookup"><span data-stu-id="d40f4-208">Reset credentials</span></span>

<span data-ttu-id="d40f4-209">Wenn Sie die Anmeldeinformationen für einen Dienstprinzipal vergessen haben, verwenden Sie [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="d40f4-209">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="d40f4-210">Der Befehl zum Zurücksetzen akzeptiert die gleichen Argumente wie `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="d40f4-210">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```

## <a name="see-also"></a><span data-ttu-id="d40f4-211">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="d40f4-211">See also</span></span>

* [<span data-ttu-id="d40f4-212">Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d40f4-212">Application and service principal objects in Azure Active Directory</span></span>](/azure/active-directory/develop/app-objects-and-service-principals)
* [<span data-ttu-id="d40f4-213">Verwalten von Dienstprinzipalen</span><span class="sxs-lookup"><span data-stu-id="d40f4-213">How to manage service principals</span></span>](/azure/developer/python/how-to-manage-service-principals)

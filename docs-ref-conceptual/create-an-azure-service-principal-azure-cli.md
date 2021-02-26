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
ms.openlocfilehash: 6b64a8f781907977d6123561d91fb8266a0ebe08
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631066"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a><span data-ttu-id="0065f-103">Erstellen eines Azure-Dienstprinzipals mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="0065f-103">Create an Azure service principal with the Azure CLI</span></span>

<span data-ttu-id="0065f-104">Für automatisierte Tools, die Azure-Dienste verwenden, sollten stets eingeschränkte Berechtigungen festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="0065f-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="0065f-105">Azure bietet Dienstprinzipale, damit Anwendungen nicht als Benutzer mit uneingeschränkten Berechtigungen angemeldet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0065f-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="0065f-106">Ein Azure-Dienstprinzipal ist eine Identität, die zur Verwendung mit Anwendungen, gehosteten Diensten und automatisierten Tools für den Zugriff auf Azure-Ressourcen erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0065f-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="0065f-107">Dieser Zugriff wird durch die dem Dienstprinzipal zugewiesenen Rollen eingeschränkt. Dadurch können Sie steuern, auf welcher Ebene auf welche Ressourcen zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="0065f-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="0065f-108">Aus Sicherheitsgründen wird stets empfohlen, Dienstprinzipale mit automatisierten Tools zu verwenden, statt ihnen die Anmeldung mit einer Benutzeridentität zu erlauben.</span><span class="sxs-lookup"><span data-stu-id="0065f-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="0065f-109">In diesem Artikel wird Schritt für Schritt erläutert, wie Sie mit der Azure CLI einen Dienstprinzipal erstellen, Informationen zu ihm abrufen und ihn zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="0065f-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="0065f-110">Erstellen eines Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="0065f-110">Create a service principal</span></span>

<span data-ttu-id="0065f-111">Erstellen Sie mit dem Befehl [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) einen Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="0065f-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="0065f-112">Beim Erstellen eines Dienstprinzipals wählen Sie den Typ der von ihm verwendeten Anmeldeauthentifizierung aus.</span><span class="sxs-lookup"><span data-stu-id="0065f-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

<span data-ttu-id="0065f-113">Für Dienstprinzipale stehen zwei Authentifizierungstypen zur Verfügung: Kennwortbasierte Authentifizierung und zertifikatbasierte Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="0065f-113">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

> [!NOTE]
>
> <span data-ttu-id="0065f-114">Wenn Ihr Konto nicht über Berechtigungen zum Erstellen eines Dienstprinzipals verfügt, gibt `az ad sp create-for-rbac` eine Fehlermeldung mit dem Hinweis „Nicht genügend Berechtigungen zum Abschließen des Vorgangs“ zurück.</span><span class="sxs-lookup"><span data-stu-id="0065f-114">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="0065f-115">Bitten Sie den Azure Active Directory-Administrator, einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0065f-115">Contact your Azure Active Directory admin to create a service principal.</span></span>

> [!WARNING]
> <span data-ttu-id="0065f-116">Wenn Sie mithilfe des Befehls `az ad sp create-for-rbac` einen Dienstprinzipal erstellen, enthält die Ausgabe Anmeldeinformationen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0065f-116">When you create a service principal using the `az ad sp create-for-rbac` command, the output includes credentials that you must protect.</span></span> <span data-ttu-id="0065f-117">Schließen Sie diese Anmeldeinformationen nicht in Ihren Code ein, und checken Sie sie nicht in Ihre Quellcodeverwaltung ein.</span><span class="sxs-lookup"><span data-stu-id="0065f-117">Be sure that you do not include these credentials in your code or check the credentials into your source control.</span></span> <span data-ttu-id="0065f-118">Verwenden Sie als Alternative ggf. [verwaltete Identitäten](/azure/active-directory/managed-identities-azure-resources/overview) (sofern verfügbar), um zu vermeiden, dass die Verwendung von Anmeldeinformationen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0065f-118">As an alternative, consider using [managed identities](/azure/active-directory/managed-identities-azure-resources/overview) if available to avoid the need to use credentials.</span></span>
>
> <span data-ttu-id="0065f-119">`az ad sp create-for-rbac` weist dem Dienstprinzipal standardmäßig auf Abonnementebene die Rolle [Mitwirkender](/azure/role-based-access-control/built-in-roles#contributor) zu.</span><span class="sxs-lookup"><span data-stu-id="0065f-119">By default, `az ad sp create-for-rbac` assigns the [Contributor](/azure/role-based-access-control/built-in-roles#contributor) role to the service principal at the subscription scope.</span></span> <span data-ttu-id="0065f-120">Um das Risiko eines kompromittierten Dienstprinzipals zu verringern, weisen Sie eine spezifischere Rolle zu, und schränken Sie den Bereich auf eine Ressource oder Ressourcengruppe ein.</span><span class="sxs-lookup"><span data-stu-id="0065f-120">To reduce your risk of a compromised service principal, assign a more specific role and narrow the scope to a resource or resource group.</span></span> <span data-ttu-id="0065f-121">Weitere Informationen finden Sie unter [Schritte zum Hinzufügen einer Rollenzuweisung](/azure/role-based-access-control/role-assignments-steps).</span><span class="sxs-lookup"><span data-stu-id="0065f-121">See [Steps to add a role assignment](/azure/role-based-access-control/role-assignments-steps) for more information.</span></span>
>
> <span data-ttu-id="0065f-122">In einem zukünftigen Release wird mit `az ad sp create-for-rbac` die Rollenzuweisung **Mitwirkender** NICHT standardmäßig erstellt.</span><span class="sxs-lookup"><span data-stu-id="0065f-122">In a future release, `az ad sp create-for-rbac` will NOT create a **Contributor** role assignment by default.</span></span> <span data-ttu-id="0065f-123">Verwenden Sie bei Bedarf das Argument `--role`, um explizit eine Rollenzuweisung zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0065f-123">If needed, use the `--role` argument to explicitly create a role assignment.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="0065f-124">Kennwortbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="0065f-124">Password-based authentication</span></span>

<span data-ttu-id="0065f-125">Ohne jegliche Authentifizierungsparameter wird die kennwortbasierte Authentifizierung mit einem für Sie erstellten zufälligen Kennwort verwendet.</span><span class="sxs-lookup"><span data-stu-id="0065f-125">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="0065f-126">Ab Azure CLI 2.0.68 wird der Parameter `--password` zum Erstellen eines Dienstprinzipals mit einem benutzerdefinierten Kennwort __nicht mehr unterstützt__, um die versehentliche Verwendung von unsicheren Kennwörtern zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="0065f-126">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="0065f-127">Die Ausgabe für einen Dienstprinzipal mit Kennwortauthentifizierung enthält den Schlüssel `password`.</span><span class="sxs-lookup"><span data-stu-id="0065f-127">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="0065f-128">Kopieren Sie diesen Wert __unbedingt__, da er nicht abgerufen werden kann.</span><span class="sxs-lookup"><span data-stu-id="0065f-128">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="0065f-129">Wenn Sie das Kennwort vergessen haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0065f-129">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="0065f-130">Die Schlüssel `appId` und `tenant` werden in der Ausgabe von `az ad sp create-for-rbac` angezeigt und bei der Dienstprinzipalauthentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="0065f-130">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="0065f-131">Notieren Sie die Werte. Sie können jedoch auch jederzeit mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-131">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="0065f-132">Zertifikatbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="0065f-132">Certificate-based authentication</span></span>

<span data-ttu-id="0065f-133">Verwenden Sie für die zertifikatbasierte Authentifizierung das Argument `--cert`.</span><span class="sxs-lookup"><span data-stu-id="0065f-133">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="0065f-134">Bei Verwendung dieses Arguments muss bereits ein Zertifikat vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="0065f-134">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="0065f-135">Vergewissern Sie sich, dass alle Tools, die diesen Dienstprinzipal verwenden, Zugriff auf den privaten Schlüssel des Zertifikats haben.</span><span class="sxs-lookup"><span data-stu-id="0065f-135">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="0065f-136">Zertifikate müssen in einem ASCII-Format vorliegen, etwa PEM, CER oder DER.</span><span class="sxs-lookup"><span data-stu-id="0065f-136">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="0065f-137">Übergeben Sie das Zertifikat als Zeichenfolge, oder verwenden Sie das Format `@path`, um das Zertifikat aus einer Datei zu laden.</span><span class="sxs-lookup"><span data-stu-id="0065f-137">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

> [!NOTE]
> <span data-ttu-id="0065f-138">Bei Verwendung einer PEM-Datei muss das Zertifikat (**CERTIFICATE**) an den privaten Schlüssel (**PRIVATE KEY**) in der Datei angefügt werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-138">When using a PEM file, the **CERTIFICATE** must be appended to the **PRIVATE KEY** within the file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="0065f-139">Das Argument `--keyvault` kann hinzugefügt werden, um ein Zertifikat in Azure Key Vault zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0065f-139">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="0065f-140">In diesem Fall ist der Wert `--cert` der Name des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="0065f-140">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="0065f-141">Verwenden Sie das Argument `--create-cert`, um ein _selbstsigniertes_ Zertifikat für die Authentifizierung zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="0065f-141">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="0065f-142">Konsolenausgabe:</span><span class="sxs-lookup"><span data-stu-id="0065f-142">Console output:</span></span>

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

<span data-ttu-id="0065f-143">Inhalt der neuen PEM-Datei:</span><span class="sxs-lookup"><span data-stu-id="0065f-143">Contents of the new PEM file:</span></span>
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> <span data-ttu-id="0065f-144">Mit dem Befehl `az ad sp create-for-rbac --create-cert` werden der Dienstprinzipal und eine PEM-Datei erstellt.</span><span class="sxs-lookup"><span data-stu-id="0065f-144">The `az ad sp create-for-rbac --create-cert` command creates the service principal and a PEM file.</span></span> <span data-ttu-id="0065f-145">Die PEM-Datei enthält einen ordnungsgemäß formatierten privaten Schlüssel (**PRIVATE KEY**) und ein ordnungsgemäß formatiertes Zertifikat (**CERTIFICATE**).</span><span class="sxs-lookup"><span data-stu-id="0065f-145">The PEM file contains a correctly formatted **PRIVATE KEY** and **CERTIFICATE**.</span></span>

<span data-ttu-id="0065f-146">Das Argument `--keyvault` kann hinzugefügt werden, um das Zertifikat in Azure Key Vault zu speichern.</span><span class="sxs-lookup"><span data-stu-id="0065f-146">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="0065f-147">Bei Verwendung von `--keyvault` ist das Argument `--cert`__erforderlich__.</span><span class="sxs-lookup"><span data-stu-id="0065f-147">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="0065f-148">Die Ausgabe enthält den Schlüssel `fileWithCertAndPrivateKey`, es sei denn, Sie speichern das Zertifikat in Key Vault.</span><span class="sxs-lookup"><span data-stu-id="0065f-148">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="0065f-149">Am Wert dieses Schlüssels können Sie erkennen, wo das generierte Zertifikat gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="0065f-149">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="0065f-150">Kopieren Sie das Zertifikat __unbedingt__ an einen sicheren Speicherort. Andernfalls können Sie sich nicht mit diesem Dienstprinzipal anmelden.</span><span class="sxs-lookup"><span data-stu-id="0065f-150">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="0065f-151">Rufen Sie für in Key Vault gespeicherte Zertifikate den privaten Schlüssel des Zertifikats mit [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show) ab.</span><span class="sxs-lookup"><span data-stu-id="0065f-151">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="0065f-152">In Key Vault ist der Name des Zertifikatgeheimnisses mit dem Zertifikatnamen identisch.</span><span class="sxs-lookup"><span data-stu-id="0065f-152">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="0065f-153">Wenn Sie keinen Zugriff mehr auf den privaten Schlüssel des Zertifikats haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0065f-153">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="0065f-154">Die Schlüssel `appId` und `tenant` werden in der Ausgabe von `az ad sp create-for-rbac` angezeigt und bei der Dienstprinzipalauthentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="0065f-154">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="0065f-155">Notieren Sie die Werte. Sie können jedoch auch jederzeit mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-155">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="0065f-156">Abrufen eines vorhandenen Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="0065f-156">Get an existing service principal</span></span>

<span data-ttu-id="0065f-157">Mit [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list) kann eine Liste der Dienstprinzipale in einem Mandanten abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-157">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="0065f-158">Dieser Befehl gibt standardmäßig die ersten 100 Dienstprinzipale für Ihren Mandanten zurück.</span><span class="sxs-lookup"><span data-stu-id="0065f-158">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="0065f-159">Verwenden Sie zum Abrufen aller Dienstprinzipale eines Mandanten das Argument `--all`.</span><span class="sxs-lookup"><span data-stu-id="0065f-159">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="0065f-160">Da das Abrufen dieser Liste sehr lange dauern kann, wird empfohlen, die Liste mit einem der folgenden Argumente zu filtern:</span><span class="sxs-lookup"><span data-stu-id="0065f-160">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="0065f-161">`--display-name` fordert Dienstprinzipale mit einem _Präfix_ an, das dem angegebenen Namen entspricht.</span><span class="sxs-lookup"><span data-stu-id="0065f-161">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="0065f-162">Der Anzeigename eines Dienstprinzipals ist der Wert, der während der Erstellung mit dem Parameter `--name` festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="0065f-162">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="0065f-163">Haben Sie `--name` während der Erstellung des Dienstprinzipals nicht festgelegt, lautet das Namenspräfix `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="0065f-163">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="0065f-164">`--spn` filtert nach genauen Übereinstimmungen des Dienstprinzipalnamens.</span><span class="sxs-lookup"><span data-stu-id="0065f-164">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="0065f-165">Der Dienstprinzipalname beginnt immer mit `https://`.</span><span class="sxs-lookup"><span data-stu-id="0065f-165">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="0065f-166">Handelte es sich bei dem für `--name` verwendeten Wert nicht um einen URI, wird für diesen Wert `https://` gefolgt vom Anzeigenamen verwendet.</span><span class="sxs-lookup"><span data-stu-id="0065f-166">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="0065f-167">`--show-mine` fordert nur Dienstprinzipale an, die vom angemeldeten Benutzer erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="0065f-167">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="0065f-168">`--filter` akzeptiert einen OData-Filter und führt die _serverseitige_ Filterung aus.</span><span class="sxs-lookup"><span data-stu-id="0065f-168">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="0065f-169">Diese Methode wird anstelle der clientseitigen Filterung mit dem Argument `--query` der CLI empfohlen.</span><span class="sxs-lookup"><span data-stu-id="0065f-169">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="0065f-170">Weitere Informationen zu OData-Filtern finden Sie unter [OData-Ausdruckssyntax für Filter und Sortierklauseln in Azure Search](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="0065f-170">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="0065f-171">Für Dienstprinzipalobjekte werden ausführliche Informationen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0065f-171">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="0065f-172">Verwenden Sie die Abfragezeichenfolge `[].{id:appId, tenant:appOwnerTenantId}`, um nur die für die Anmeldung erforderlichen Informationen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="0065f-172">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="0065f-173">Die Anmeldeinformationen für alle Dienstprinzipale, die vom derzeit angemeldeten Benutzer erstellt wurden, rufen Sie beispielsweise wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="0065f-173">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="0065f-174">Mit `az ad sp list` und [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) rufen Sie den Benutzer und den Mandanten ab, allerdings nicht die Authentifizierungsgeheimnisse _oder_ die Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="0065f-174">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="0065f-175">Geheimnisse für Zertifikate in Key Vault können mit [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show) abgerufen werden. Andere Geheimnisse werden jedoch nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="0065f-175">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="0065f-176">Wenn Sie eine Authentifizierungsmethode oder ein Geheimnis vergessen haben, [setzen Sie die Anmeldeinformationen des Dienstprinzipals zurück](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0065f-176">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="0065f-177">Verwalten von Dienstprinzipalrollen</span><span class="sxs-lookup"><span data-stu-id="0065f-177">Manage service principal roles</span></span>

<span data-ttu-id="0065f-178">Die Azure CLI enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:</span><span class="sxs-lookup"><span data-stu-id="0065f-178">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="0065f-179">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="0065f-179">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="0065f-180">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="0065f-180">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="0065f-181">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="0065f-181">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="0065f-182">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="0065f-182">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="0065f-183">Diese Rolle besitzt uneingeschränkte Berechtigungen für Lese- und Schreibvorgänge in einem Azure-Konto.</span><span class="sxs-lookup"><span data-stu-id="0065f-183">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="0065f-184">Die Rolle **Leser** ist stärker eingeschränkt und bietet schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="0065f-184">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="0065f-185">Weitere Informationen zur rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) finden Sie unter [Rollenbasierte Zugriffssteuerung: Integrierte Rollen](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="0065f-185">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="0065f-186">Das folgende Beispiel fügt die Rolle **Leser** hinzu und entfernt die Rolle **Mitwirkender**:</span><span class="sxs-lookup"><span data-stu-id="0065f-186">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="0065f-187">Wenn Ihr Konto nicht über Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ hat. Bitten Sie den Azure Active Directory-Administrator um die Verwaltung von Rollen.</span><span class="sxs-lookup"><span data-stu-id="0065f-187">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="0065f-188">Durch das Hinzufügen einer Rolle werden zuvor zugewiesene Berechtigungen _nicht_ eingeschränkt.</span><span class="sxs-lookup"><span data-stu-id="0065f-188">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="0065f-189">Beim Einschränken der Berechtigungen eines Dienstprinzipals sollte die Rolle __Mitwirkender__ entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-189">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="0065f-190">Die Änderungen können durch Auflisten der zugewiesenen Rollen überprüft werden:</span><span class="sxs-lookup"><span data-stu-id="0065f-190">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="0065f-191">Anmelden mithilfe eines Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="0065f-191">Sign in using a service principal</span></span>

<span data-ttu-id="0065f-192">Testen Sie die Anmeldeinformationen und Berechtigungen des neuen Dienstprinzipals, indem Sie sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="0065f-192">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="0065f-193">Für die Anmeldung mit einem Dienstprinzipal benötigen Sie `appId`, `tenant` und Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="0065f-193">To sign in with a service principal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="0065f-194">So melden Sie sich mit einem Dienstprinzipal und einem Kennwort an:</span><span class="sxs-lookup"><span data-stu-id="0065f-194">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="0065f-195">Um sich mit einem Zertifikat anmelden zu können, muss es lokal als PEM- oder DER-Datei im ASCII-Format verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="0065f-195">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format.</span></span> <span data-ttu-id="0065f-196">Bei Verwendung einer PEM-Datei müssen der private Schlüssel (**PRIVATE KEY**) und das Zertifikat (**CERTIFICATE**) gemeinsam innerhalb der Datei angefügt werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-196">When using a PEM file, the **PRIVATE KEY** and **CERTIFICATE** must be appended together within the file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="0065f-197">Weitere Informationen zum Anmelden mit einem Dienstprinzipal finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0065f-197">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="create-a-resource-using-service-principal"></a><span data-ttu-id="0065f-198">Erstellen einer Ressource mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="0065f-198">Create a resource using service principal</span></span>

<span data-ttu-id="0065f-199">Der folgende Abschnitt enthält ein Beispiel für die Erstellung einer Ressource für [Azure Storage](/azure/storage/) mit einem Dienstprinzipal. Dazu werden die folgenden Befehle verwendet:</span><span class="sxs-lookup"><span data-stu-id="0065f-199">The following section provides an example of how to create an resource for [Azure Storage](/azure/storage/) with a service principal, using the following commands:</span></span>

* [<span data-ttu-id="0065f-200">az login</span><span class="sxs-lookup"><span data-stu-id="0065f-200">az login</span></span>](/cli/azure/reference-index#az_login)
* [<span data-ttu-id="0065f-201">az group create</span><span class="sxs-lookup"><span data-stu-id="0065f-201">az group create</span></span>](/cli/azure/group#az_group_create)
* [<span data-ttu-id="0065f-202">az storage account create</span><span class="sxs-lookup"><span data-stu-id="0065f-202">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)
* [<span data-ttu-id="0065f-203">az storage account keys list</span><span class="sxs-lookup"><span data-stu-id="0065f-203">az storage account keys list</span></span>](/cli/azure/storage/account/keys#az_storage_account_keys_list)

<span data-ttu-id="0065f-204">Für die Anmeldung mit einem Dienstprinzipal benötigen Sie die Werte für `appId`, `tenant` und `password`, die beim [Erstellen des Dienstprinzipals](#sign-in-using-a-service-principal) als Antwort zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="0065f-204">To sign in with a service principal, you need the `appId`, `tenant`, and `password` returned as the response when you [created your service principal](#sign-in-using-a-service-principal).</span></span>

1. <span data-ttu-id="0065f-205">Melden Sie sich als Dienstprinzipal an.</span><span class="sxs-lookup"><span data-stu-id="0065f-205">Log in as the service principal.</span></span>

    ```azurecli-interactive
    az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
    ```

1. <span data-ttu-id="0065f-206">Erstellen Sie eine Ressourcengruppe für alle Ressourcen, die für den gleichen Schnellstart, das gleiche Tutorial oder das gleiche Entwicklungsprojekt verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="0065f-206">Create a resource group to hold all resources used for the same quickstart, tutorial, or development project.</span></span>

    ```azurecli-interactive
    az group create --location WESTUS --name MY_RESOURCE_GROUP
    ```

1. <span data-ttu-id="0065f-207">Erstellen Sie eine Ressource für einen Azure-Dienst.</span><span class="sxs-lookup"><span data-stu-id="0065f-207">Create a resource to an Azure service.</span></span> <span data-ttu-id="0065f-208">Ersetzen Sie `<SERVICENAME>` durch den Namen des Azure-Diensts.</span><span class="sxs-lookup"><span data-stu-id="0065f-208">Replace `<SERVICENAME>` with the name of the Azure service.</span></span>

    <span data-ttu-id="0065f-209">Für Azure Storage sind folgende Werte für den Parameter `<KIND>` zulässig:</span><span class="sxs-lookup"><span data-stu-id="0065f-209">For Azure Storage, valid values for the `<KIND>` parameter are:</span></span>

    * <span data-ttu-id="0065f-210">BlobStorage</span><span class="sxs-lookup"><span data-stu-id="0065f-210">BlobStorage</span></span>
    * <span data-ttu-id="0065f-211">BlockBlobStorage</span><span class="sxs-lookup"><span data-stu-id="0065f-211">BlockBlobStorage</span></span>
    * <span data-ttu-id="0065f-212">FileStorage</span><span class="sxs-lookup"><span data-stu-id="0065f-212">FileStorage</span></span>
    * <span data-ttu-id="0065f-213">Storage</span><span class="sxs-lookup"><span data-stu-id="0065f-213">Storage</span></span>
    * <span data-ttu-id="0065f-214">StorageV2</span><span class="sxs-lookup"><span data-stu-id="0065f-214">StorageV2</span></span>

    ```azurecli-interactive
    az storage account create --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP --kind <KIND> --sku F0 --location WESTUS --yes
    ```

1. <span data-ttu-id="0065f-215">Rufen Sie Ressourcenschlüssel für die neue Ressource ab. Sie verwenden ihn in Ihrem Code zum Authentifizieren beim Azure-Dienst.</span><span class="sxs-lookup"><span data-stu-id="0065f-215">Get resource keys for the new resource, which you use in your code to authenticate to the Azure service.</span></span>

    ```azurecli-interactive
    az storage account keys list --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP
    ```

## <a name="reset-credentials"></a><span data-ttu-id="0065f-216">Zurücksetzen von Anmeldeinformation</span><span class="sxs-lookup"><span data-stu-id="0065f-216">Reset credentials</span></span>

<span data-ttu-id="0065f-217">Wenn Sie die Anmeldeinformationen für einen Dienstprinzipal vergessen haben, verwenden Sie [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="0065f-217">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="0065f-218">Der Befehl zum Zurücksetzen akzeptiert die gleichen Argumente wie `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="0065f-218">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```

## <a name="see-also"></a><span data-ttu-id="0065f-219">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="0065f-219">See also</span></span>

* [<span data-ttu-id="0065f-220">Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0065f-220">Application and service principal objects in Azure Active Directory</span></span>](/azure/active-directory/develop/app-objects-and-service-principals)
* [<span data-ttu-id="0065f-221">Verwalten von Dienstprinzipalen</span><span class="sxs-lookup"><span data-stu-id="0065f-221">How to manage service principals</span></span>](/azure/developer/python/how-to-manage-service-principals)

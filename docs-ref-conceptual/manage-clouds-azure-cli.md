---
title: Verwalten mehrerer Clouds mit der Azure CLI 2.0
description: Die Azure CLI 2.0 ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei mehreren Clouds.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 836bf920adaae7bff8482c697bf105f0d457c658
ms.sourcegitcommit: fb3fed8701aff6c46af856e8fdc3e56ff9a678bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38228936"
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="b2114-103">Verwalten mehrerer Clouds mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="b2114-103">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="b2114-104">Wenn Sie regionsübergreifend arbeiten oder [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/) verwenden, müssen Sie möglicherweise mehrere Clouds verwenden.</span><span class="sxs-lookup"><span data-stu-id="b2114-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="b2114-105">Hierzu stellt Ihnen Microsoft Clouds zur Verfügung, die mit regionalen Gesetzen in Einklang stehen.</span><span class="sxs-lookup"><span data-stu-id="b2114-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="b2114-106">In diesem Artikel erfahren Sie, wie Sie Informationen zu Clouds abrufen, die für Ihr Konto verfügbar sind, wie Sie die aktuelle Cloud ändern und wie Sie neue Clouds für die Verwendung mit Azure Stack registrieren bzw. die Registrierung aufheben.</span><span class="sxs-lookup"><span data-stu-id="b2114-106">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="b2114-107">Auflisten von Clouds</span><span class="sxs-lookup"><span data-stu-id="b2114-107">Listing clouds</span></span>

<span data-ttu-id="b2114-108">Die verfügbaren Clouds können mit dem Befehl [az cloud list](/cli/azure/cloud#az-cloud-list) aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="b2114-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="b2114-109">So erfahren Sie, welche Cloud derzeit aktiv ist, und erhalten Informationen zum aktuellen Profil, zu regionalen Suffixen und zu Hostnamen.</span><span class="sxs-lookup"><span data-stu-id="b2114-109">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="b2114-110">Gehen Sie wie folgt vor, um die aktive Cloud und eine Liste mit allen verfügbaren Clouds abzurufen:</span><span class="sxs-lookup"><span data-stu-id="b2114-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

<span data-ttu-id="b2114-111">Für die derzeit aktive Cloud ist in der Spalte `IsActive` der Wert `True` angegeben.</span><span class="sxs-lookup"><span data-stu-id="b2114-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="b2114-112">Es kann immer nur eine Cloud aktiv sein.</span><span class="sxs-lookup"><span data-stu-id="b2114-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="b2114-113">Ausführlichere Informationen zu einer Cloud (einschließlich der Endpunkte, die sie für Azure-Dienste verwendet) erhalten Sie mit dem Befehl `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="b2114-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a><span data-ttu-id="b2114-114">Wechseln der aktiven Cloud</span><span class="sxs-lookup"><span data-stu-id="b2114-114">Switching the active cloud</span></span>

<span data-ttu-id="b2114-115">Führen Sie zum Wechseln der aktiven Cloud den Befehl [az cloud set](/cli/azure/cloud#az-cloud-set) aus.</span><span class="sxs-lookup"><span data-stu-id="b2114-115">To switch the currently active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="b2114-116">Dieser Befehl erfordert ein Argument: den Namen der Cloud.</span><span class="sxs-lookup"><span data-stu-id="b2114-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="b2114-117">Sollte die Authentifizierung für die aktivierte Cloud abgelaufen sein, müssen Sie sich erneut authentifizieren, bevor Sie weitere CLI-Aufgaben ausführen.</span><span class="sxs-lookup"><span data-stu-id="b2114-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="b2114-118">Beim erstmaligen Wechsel zu der neuen Cloud muss auch das aktive Abonnement festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b2114-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="b2114-119">Anleitungen zur Authentifizierung finden Sie unter [Anmelden bei der Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b2114-119">For instructions on authenticating, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="b2114-120">Weitere Informationen zur Abonnementverwaltung finden Sie unter [Verwalten mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b2114-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="b2114-121">Registrieren einer Cloud</span><span class="sxs-lookup"><span data-stu-id="b2114-121">Register a cloud</span></span>

<span data-ttu-id="b2114-122">Registrieren Sie eine neue Cloud, wenn Sie über eigene Endpunkte für Azure Stack verfügen.</span><span class="sxs-lookup"><span data-stu-id="b2114-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="b2114-123">Eine Cloud wird mit dem Befehl [az cloud register](/cli/azure/cloud#az-cloud-register) erstellt.</span><span class="sxs-lookup"><span data-stu-id="b2114-123">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="b2114-124">Dieser Befehl erfordert einen Namen und einen Satz von Funktionen mit den dazugehörigen Endpunkten.</span><span class="sxs-lookup"><span data-stu-id="b2114-124">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="b2114-125">Informationen zum Registrieren einer Cloud für die Verwendung mit Azure Stack finden Sie unter [Verwenden von API-Versionsprofilen mit Azure CLI 2.0 in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="b2114-125">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI 2.0 in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="b2114-126">Für China, US Government oder deutsche Regionen müssen Sie Ihre eigene Cloud nicht registrieren.</span><span class="sxs-lookup"><span data-stu-id="b2114-126">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="b2114-127">Diese werden von Microsoft verwaltet und sind standardmäßig verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b2114-127">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="b2114-128">Weitere Informationen zu allen verfügbaren Endpunkteinstellungen finden Sie in der [Dokumentation für `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="b2114-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="b2114-129">Durch Registrieren einer Cloud wird nicht automatisch zu dieser Cloud gewechselt.</span><span class="sxs-lookup"><span data-stu-id="b2114-129">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="b2114-130">Wählen Sie die neu erstellte Cloud wie weiter oben beschrieben mithilfe des Befehls `az cloud set` aus.</span><span class="sxs-lookup"><span data-stu-id="b2114-130">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="b2114-131">Aktualisieren einer vorhandenen Cloud</span><span class="sxs-lookup"><span data-stu-id="b2114-131">Update an existing cloud</span></span>

<span data-ttu-id="b2114-132">Sie können auch eine vorhandene Cloud aktualisieren, sofern Sie über die erforderlichen Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="b2114-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="b2114-133">Führen Sie diesen Schritt aus, wenn Sie zu einem anderen Azure-Profil wechseln oder einen Endpunkt hinzufügen oder ändern müssen.</span><span class="sxs-lookup"><span data-stu-id="b2114-133">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="b2114-134">Verwenden Sie dazu den Befehl [az cloud update](/cli/azure/cloud#az-cloud-update). Dieser akzeptiert die gleichen Argumente wie `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="b2114-134">You do this with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="b2114-135">Aufheben der Registrierung einer Cloud</span><span class="sxs-lookup"><span data-stu-id="b2114-135">Unregister a cloud</span></span>

<span data-ttu-id="b2114-136">Wenn Sie eine registrierte Cloud nicht mehr benötigen, können Sie die Registrierung mit dem Befehl [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) aufheben:</span><span class="sxs-lookup"><span data-stu-id="b2114-136">If you no longer require a registered cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```

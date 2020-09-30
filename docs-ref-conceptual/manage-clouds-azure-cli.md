---
title: Auswählen von Clouds mit der Azure CLI
description: Die Azure CLI ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei mehreren Clouds.
author: dbradish-microsoft
manager: barbkess
ms.author: dbradish
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: b59da347069f0df61756eac958c6a0119a31be18
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225319"
---
# <a name="select-clouds-with-the-azure-cli"></a><span data-ttu-id="b0ceb-103">Auswählen von Clouds mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b0ceb-103">Select clouds with the Azure CLI</span></span>

<span data-ttu-id="b0ceb-104">Wenn Sie regionsübergreifend arbeiten oder [Azure Stack](/azure/azure-stack/user/) verwenden, müssen Sie möglicherweise mehrere Clouds verwenden.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-104">If you work across different regions or use [Azure Stack](/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="b0ceb-105">Hierzu stellt Ihnen Microsoft Clouds zur Verfügung, die mit regionalen Gesetzen in Einklang stehen.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="b0ceb-106">In diesem Artikel erfahren Sie, wie Sie Informationen zu Clouds abrufen, wie Sie die aktuelle Cloud ändern und wie Sie neue Clouds registrieren bzw. ihre Registrierung aufheben.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="b0ceb-107">Auflisten verfügbarer Clouds</span><span class="sxs-lookup"><span data-stu-id="b0ceb-107">List available clouds</span></span>

<span data-ttu-id="b0ceb-108">Die verfügbaren Clouds können mit dem Befehl [az cloud list](/cli/azure/cloud#az-cloud-list) aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="b0ceb-109">Mit diesem Befehl erfahren Sie, welche Cloud derzeit aktiv ist, und erhalten Informationen zum aktuellen Profil, zu regionalen Suffixen und zu Hostnamen.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="b0ceb-110">Gehen Sie wie folgt vor, um die aktive Cloud und eine Liste mit allen verfügbaren Clouds abzurufen:</span><span class="sxs-lookup"><span data-stu-id="b0ceb-110">To get the active cloud and a list of all the available clouds:</span></span>

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

<span data-ttu-id="b0ceb-111">Für die derzeit aktive Cloud ist in der Spalte `IsActive` der Wert `True` angegeben.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="b0ceb-112">Es kann immer nur eine Cloud aktiv sein.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="b0ceb-113">Ausführlichere Informationen zu einer Cloud (einschließlich der Endpunkte, die sie für Azure-Dienste verwendet) erhalten Sie mit dem Befehl `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="b0ceb-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```json
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

## <a name="switch-the-active-cloud"></a><span data-ttu-id="b0ceb-114">Wechseln der aktiven Cloud</span><span class="sxs-lookup"><span data-stu-id="b0ceb-114">Switch the active cloud</span></span>

<span data-ttu-id="b0ceb-115">Informationen zum Festlegen der Standardcloud mithilfe einer Konfigurationsdatei finden Sie unter [CLI-Konfigurationswerte und Umgebungsvariablen](./azure-cli-configuration.md?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span><span class="sxs-lookup"><span data-stu-id="b0ceb-115">To set the default cloud using a configuration file, see [CLI configuration values and environment variables](./azure-cli-configuration.md?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span></span>  <span data-ttu-id="b0ceb-116">Führen Sie zum Wechseln der Cloud den Befehl [az cloud set](/cli/azure/cloud#az-cloud-set) aus.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-116">To switch the active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="b0ceb-117">Dieser Befehl erfordert ein Argument: den Namen der Cloud.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="b0ceb-118">Sollte die Authentifizierung für die aktivierte Cloud abgelaufen sein, müssen Sie sich erneut authentifizieren, bevor Sie weitere CLI-Aufgaben ausführen.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="b0ceb-119">Beim erstmaligen Wechsel zu der neuen Cloud muss auch das aktive Abonnement festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="b0ceb-120">Eine Anleitung zur Authentifizierung finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b0ceb-120">For instructions on authenticating, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span> <span data-ttu-id="b0ceb-121">Weitere Informationen zur Abonnementverwaltung finden Sie unter [Verwalten von Azure-Abonnements mit der Azure CLI](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b0ceb-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="b0ceb-122">Registrieren einer neuen Cloud</span><span class="sxs-lookup"><span data-stu-id="b0ceb-122">Register a new cloud</span></span>

<span data-ttu-id="b0ceb-123">Registrieren Sie eine neue Cloud, wenn Sie über eigene Endpunkte für Azure Stack verfügen.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="b0ceb-124">Eine Cloud wird mit dem Befehl [az cloud register](/cli/azure/cloud#az-cloud-register) erstellt.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-124">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="b0ceb-125">Dieser Befehl erfordert einen Namen und eine Reihe von Dienstendpunkten.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-125">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="b0ceb-126">Informationen zum Registrieren einer Cloud für die Verwendung mit Azure Stack finden Sie unter [Verwenden von API-Versionsprofilen mit der Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="b0ceb-126">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="b0ceb-127">Für China, US Government oder deutsche Regionen müssen Sie keine Informationen registrieren.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-127">You don't need to register information for the China, US Government, or German regions.</span></span> <span data-ttu-id="b0ceb-128">Diese Clouds werden von Microsoft verwaltet und sind standardmäßig verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-128">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="b0ceb-129">Weitere Informationen zu allen verfügbaren Endpunkteinstellungen finden Sie in der [Dokumentation für `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="b0ceb-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="b0ceb-130">Durch Registrieren einer Cloud wird nicht automatisch zu dieser Cloud gewechselt.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-130">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="b0ceb-131">Wählen Sie die neu erstellte Cloud mithilfe des Befehls `az cloud set` aus.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-131">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="b0ceb-132">Aktualisieren einer vorhandenen Cloud</span><span class="sxs-lookup"><span data-stu-id="b0ceb-132">Update an existing cloud</span></span>

<span data-ttu-id="b0ceb-133">Sie können auch eine vorhandene Cloud aktualisieren, sofern Sie über die erforderlichen Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="b0ceb-134">Bei der Aktualisierung einer Cloud wird zu einem anderen Azure-Dienstprofil gewechselt, oder die Verbindungsendpunkte werden geändert.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-134">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="b0ceb-135">Aktualisieren Sie eine Cloud mit dem Befehl [az cloud update](/cli/azure/cloud#az-cloud-update). Dieser akzeptiert die gleichen Argumente wie `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="b0ceb-135">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="b0ceb-136">Aufheben der Registrierung einer Cloud</span><span class="sxs-lookup"><span data-stu-id="b0ceb-136">Unregister a cloud</span></span>

<span data-ttu-id="b0ceb-137">Wenn Sie eine erstellte Cloud nicht mehr benötigen, kann ihre Registrierung mit dem Befehl [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) aufgehoben werden:</span><span class="sxs-lookup"><span data-stu-id="b0ceb-137">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```
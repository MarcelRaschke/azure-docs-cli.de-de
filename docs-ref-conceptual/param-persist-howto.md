---
title: 'Permanente Azure CLI-Parameter: Optionen'
description: 'Gewusst wie: Verwenden von permanenten Azure CLI-Parametern zum Speichern von wiederverwendbaren Parameterwerten'
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: bfaf414ab03482fb1bae7da98ddb517435f331ee
ms.sourcegitcommit: 4c41593455b473c796735c73590403d9b6be87a2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/05/2021
ms.locfileid: "99572764"
---
# <a name="azure-cli-persisted-parameter"></a><span data-ttu-id="9fe07-103">Permanente Azure CLI-Parameter</span><span class="sxs-lookup"><span data-stu-id="9fe07-103">Azure CLI persisted parameter</span></span>

<span data-ttu-id="9fe07-104">Mit dem Azure CLI-Referenzbefehl [az config param-persist](/cli/azure/param-persist) können lokale permanente Parameterwerte für Azure CLI-Befehle festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="9fe07-104">The Azure CLI [az config param-persist](/cli/azure/param-persist) reference provides the ability to retain local persisted parameter values for Azure CLI commands.</span></span>  <span data-ttu-id="9fe07-105">Es ist dann nicht mehr erforderlich, häufig verwendete Parameter ständig neu einzugeben.</span><span class="sxs-lookup"><span data-stu-id="9fe07-105">This removes the need to continually retype common parameters.</span></span> <span data-ttu-id="9fe07-106">Beispielsweise sind die Parameter für den Speicherort (location) und die Ressourcengruppe (resource-group) in vielen CLI-Befehlen erforderlich, aber sie tragen nicht zur _Absicht_ des Befehls bei.</span><span class="sxs-lookup"><span data-stu-id="9fe07-106">For example, location and resource-group are required parameters in many CLI commands, but they don't contribute to the _intent_ of the command.</span></span>  <span data-ttu-id="9fe07-107">Wenn Sie Parameterwerte mit permanenten Parametern speichern, verringern Sie die Redundanz und können die CLI-Befehlssyntax deutlich verkürzen.</span><span class="sxs-lookup"><span data-stu-id="9fe07-107">When you store parameter values with persisted parameter, you reduce redundancy and can significantly shorten CLI command syntax.</span></span>

<span data-ttu-id="9fe07-108">Von der CLI verwendete Konfigurationswerte werden in der folgenden Reihenfolge ausgewertet. Die Liste ist nach absteigender Priorität sortiert.</span><span class="sxs-lookup"><span data-stu-id="9fe07-108">Configuration values used by the CLI are evaluated in the following precedence, with items higher on the list taking priority.</span></span>

1. <span data-ttu-id="9fe07-109">Befehlszeilenparameter</span><span class="sxs-lookup"><span data-stu-id="9fe07-109">Command-line parameters</span></span>
1. <span data-ttu-id="9fe07-110">Werte im lokalen Arbeitsverzeichnis, die mit `az config param-persist` festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="9fe07-110">Values in the local working directory set by `az config param-persist`</span></span>
1. <span data-ttu-id="9fe07-111">Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="9fe07-111">Environment variables</span></span>
1. <span data-ttu-id="9fe07-112">In der Konfigurationsdatei enthaltene oder mit `az config` festgelegte Werte</span><span class="sxs-lookup"><span data-stu-id="9fe07-112">Values in the configuration file or set with `az config`</span></span>

<span data-ttu-id="9fe07-113">[Installieren Sie die Azure CLI](install-azure-cli.md), oder öffnen Sie [Azure Cloud Shell](https://shell.azure.com), um die Skripts in diesem Artikel auszuführen.</span><span class="sxs-lookup"><span data-stu-id="9fe07-113">[Install the Azure CLI](install-azure-cli.md) or open [Azure Cloud Shell](https://shell.azure.com) to run the scripts in this article.</span></span>  <span data-ttu-id="9fe07-114">Wenn Sie eine lokale Installation der Azure CLI verwenden, benötigen Sie für `az config param-persist`-Befehle Version 2.12.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="9fe07-114">If you are using a local install of the Azure CLI, version 2.12.0 or later is needed to run `az config param-persist` commands.</span></span>  <span data-ttu-id="9fe07-115">Führen Sie [az version](/cli/azure/reference-index#az_version) aus, um die installierte Version und die abhängigen Bibliotheken zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="9fe07-115">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="9fe07-116">Führen Sie [az upgrade](/cli/azure/reference-index#az_upgrade) aus, um das Upgrade auf die aktuelle Version durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="9fe07-116">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>  <span data-ttu-id="9fe07-117">Azure Cloud Shell verfügt immer über die neueste Version der Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="9fe07-117">Azure Cloud Shell always has the latest version of the Azure CLI.</span></span>

## <a name="persisted-parameter-data-file"></a><span data-ttu-id="9fe07-118">Datendatei für permanente Parameter</span><span class="sxs-lookup"><span data-stu-id="9fe07-118">Persisted parameter data file</span></span>

<span data-ttu-id="9fe07-119">Permanente Parameterwerte sind in einer Datei mit dem Namen `.param_persist` enthalten, die in Ihrem Arbeitsverzeichnis gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="9fe07-119">Persisted parameter values are kept in a file named `.param_persist` which is stored in your working directory.</span></span>  <span data-ttu-id="9fe07-120">Bei Verwendung von [Azure Cloud Shell](https://shell.azure.com) zum Ausführen von Azure CLI-Befehlen befindet sich Ihr Arbeitsverzeichnis unter dem Speicherkonto, das von der Azure CLI verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9fe07-120">If you are using [Azure Cloud Shell](https://shell.azure.com) to execute Azure CLI commands, your working directory is in the storage account being used by the Azure CLI.</span></span>  <span data-ttu-id="9fe07-121">Wenn Sie eine [lokale Installation](/install-azure-cli) der Azure CLI verwenden, befindet sich Ihr Arbeitsverzeichnis auf Ihrem lokalen Computer.</span><span class="sxs-lookup"><span data-stu-id="9fe07-121">If you are using a [local install](/install-azure-cli) of the Azure CLI, your working directory is on your local machine.</span></span>  <span data-ttu-id="9fe07-122">An beiden Speicherorten ist die Datei `.param_persist` ausgeblendet und sollte nicht manuell aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="9fe07-122">In either location, the `.param_persist` file is hidden and should not be manually updated.</span></span>

## <a name="persisted-parameter-storage-and-support"></a><span data-ttu-id="9fe07-123">Speicherung und Unterstützung von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="9fe07-123">Persisted parameter storage and support</span></span>

<span data-ttu-id="9fe07-124">Die folgenden Azure CLI-Parameter werden als permanente Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fe07-124">The following Azure CLI parameters are supported by persisted parameter.</span></span>  <span data-ttu-id="9fe07-125">Die Parameter `resource_group_name` und `location` werden auf andere Weise gespeichert, damit Sie sie als permanente Parameter festlegen können, _ohne_ einen Erstellungsbefehl auszuführen.</span><span class="sxs-lookup"><span data-stu-id="9fe07-125">The `resource_group_name` and `location` parameters are stored differently in that you can add them to persisted parameter _without_ executing a create command.</span></span>

| <span data-ttu-id="9fe07-126">Permanente Parameter</span><span class="sxs-lookup"><span data-stu-id="9fe07-126">Persisted parameter</span></span> | <span data-ttu-id="9fe07-127">Speicheraktion</span><span class="sxs-lookup"><span data-stu-id="9fe07-127">Storage action</span></span> | <span data-ttu-id="9fe07-128">Unterstützt von</span><span class="sxs-lookup"><span data-stu-id="9fe07-128">Supported by</span></span>
|-|-|-|
| <span data-ttu-id="9fe07-129">location</span><span class="sxs-lookup"><span data-stu-id="9fe07-129">location</span></span> | <span data-ttu-id="9fe07-130">Ausführung eines beliebigen Befehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-130">Execute any command</span></span> | <span data-ttu-id="9fe07-131">Alle Azure CLI-Referenzbefehle</span><span class="sxs-lookup"><span data-stu-id="9fe07-131">All Azure CLI references</span></span>
| <span data-ttu-id="9fe07-132">resource_group_name</span><span class="sxs-lookup"><span data-stu-id="9fe07-132">resource_group_name</span></span> | <span data-ttu-id="9fe07-133">Ausführung eines beliebigen Befehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-133">Execute any command</span></span> | <span data-ttu-id="9fe07-134">Alle Azure CLI-Referenzbefehle</span><span class="sxs-lookup"><span data-stu-id="9fe07-134">All Azure CLI references</span></span>
| <span data-ttu-id="9fe07-135">vnet_name</span><span class="sxs-lookup"><span data-stu-id="9fe07-135">vnet_name</span></span> | <span data-ttu-id="9fe07-136">Ausführung eines Erstellungsbefehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-136">Execute a create command</span></span> | <span data-ttu-id="9fe07-137">Nur Azure-Web-Apps</span><span class="sxs-lookup"><span data-stu-id="9fe07-137">Azure Web Apps only</span></span>
| <span data-ttu-id="9fe07-138">storage_account_name</span><span class="sxs-lookup"><span data-stu-id="9fe07-138">storage_account_name</span></span> | <span data-ttu-id="9fe07-139">Ausführung eines Erstellungsbefehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-139">Execute a create command</span></span> |  <span data-ttu-id="9fe07-140">Nur Azure-Web-Apps</span><span class="sxs-lookup"><span data-stu-id="9fe07-140">Azure Web Apps only</span></span>
| <span data-ttu-id="9fe07-141">webapp_name</span><span class="sxs-lookup"><span data-stu-id="9fe07-141">webapp_name</span></span> | <span data-ttu-id="9fe07-142">Ausführung eines Erstellungsbefehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-142">Execute a create command</span></span> | <span data-ttu-id="9fe07-143">Nur Azure-Web-Apps</span><span class="sxs-lookup"><span data-stu-id="9fe07-143">Azure Web Apps only</span></span>
| <span data-ttu-id="9fe07-144">function_app_name</span><span class="sxs-lookup"><span data-stu-id="9fe07-144">function_app_name</span></span> | <span data-ttu-id="9fe07-145">Ausführung eines Erstellungsbefehls</span><span class="sxs-lookup"><span data-stu-id="9fe07-145">Execute a create command</span></span> | <span data-ttu-id="9fe07-146">Nur Azure Functions</span><span class="sxs-lookup"><span data-stu-id="9fe07-146">Azure Functions only</span></span>

## <a name="sample-script-using-persisted-parameters"></a><span data-ttu-id="9fe07-147">Beispielskript mit permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="9fe07-147">Sample script using persisted parameters</span></span>

<span data-ttu-id="9fe07-148">Ohne permanente Parameter müssen für sequenzielle CLI-Befehle die gleichen Parameterwerte immer wieder angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9fe07-148">Without persisted parameters, sequential CLI commands must repeat the same parameter values.</span></span>  <span data-ttu-id="9fe07-149">Bei aktivierten permanenten Parametern können Ihre gespeicherten Parameterwerte in sequenziellen Befehlen weggelassen werden.</span><span class="sxs-lookup"><span data-stu-id="9fe07-149">With persisted parameters enabled, your stored parameter values can be omitted from sequential commands.</span></span>  <span data-ttu-id="9fe07-150">In diesem Beispiel werden der `location`, der `resource group name` oder der `storage account name` in den nachfolgenden Befehlen wiederholt.</span><span class="sxs-lookup"><span data-stu-id="9fe07-150">In this example, the `location`, `resource group name` or `storage account name` are repeated in subsequent commands.</span></span>

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a><span data-ttu-id="9fe07-151">Vergleich zwischen permanenten Parametern und globalen Variablen</span><span class="sxs-lookup"><span data-stu-id="9fe07-151">Persisted parameter and global variable comparison</span></span>

<span data-ttu-id="9fe07-152">Es gibt zwei Azure CLI-Befehle, die als Standardparameterwerte verwendet werden können: `az configure` und `az config param-persist`.</span><span class="sxs-lookup"><span data-stu-id="9fe07-152">There are two Azure CLI commands that can be used to default parameter values: `az configure` and `az config param-persist`.</span></span>  <span data-ttu-id="9fe07-153">Verwenden Sie den Befehl `az configure`, um _globale Variablen_ anzugeben, z. B. Gruppe, Speicherort oder Web.</span><span class="sxs-lookup"><span data-stu-id="9fe07-153">Use the `az configure` command to specify _global variables_ such as group, location, or web.</span></span>  <span data-ttu-id="9fe07-154">Verwenden Sie `az param-persist`, um _lokale Standardwerte_ anzugeben, die für Ihre Workload eindeutig sind.</span><span class="sxs-lookup"><span data-stu-id="9fe07-154">Use `az param-persist` to specify _local default values_ unique to your workload.</span></span>  <span data-ttu-id="9fe07-155">Gespeicherte Werte werden von der CLI anstelle von erforderlichen Argumenten verwendet.</span><span class="sxs-lookup"><span data-stu-id="9fe07-155">Stored values are used by the CLI in place of required arguments.</span></span>

> [!Important]
> <span data-ttu-id="9fe07-156">Globale Kontextwerte werden durch permanente Parameter außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="9fe07-156">Persisted parameters override global context values.</span></span>
>

| <span data-ttu-id="9fe07-157">Verweis</span><span class="sxs-lookup"><span data-stu-id="9fe07-157">Reference</span></span> | <span data-ttu-id="9fe07-158">`Scope`</span><span class="sxs-lookup"><span data-stu-id="9fe07-158">Scope</span></span> | <span data-ttu-id="9fe07-159">Set</span><span class="sxs-lookup"><span data-stu-id="9fe07-159">Set</span></span> | <span data-ttu-id="9fe07-160">Zweck</span><span class="sxs-lookup"><span data-stu-id="9fe07-160">Use</span></span>
|-|-|-|-|
[<span data-ttu-id="9fe07-161">az configure</span><span class="sxs-lookup"><span data-stu-id="9fe07-161">az configure</span></span>](/cli/azure/reference-index#az_configure) | <span data-ttu-id="9fe07-162">Globale Gültigkeit für die gesamte CLI</span><span class="sxs-lookup"><span data-stu-id="9fe07-162">Scoped globally across the CLI</span></span> | <span data-ttu-id="9fe07-163">Explizite Festlegung mit `az configure --defaults`</span><span class="sxs-lookup"><span data-stu-id="9fe07-163">Set explicitly using `az configure --defaults`</span></span> | <span data-ttu-id="9fe07-164">Verwendung für Einstellungen, z. B. Protokollierung, Datensammlung und Standardargumentwerte</span><span class="sxs-lookup"><span data-stu-id="9fe07-164">Use for settings such as logging, data collection, and default argument values</span></span>
[<span data-ttu-id="9fe07-165">az config param-persist</span><span class="sxs-lookup"><span data-stu-id="9fe07-165">az config param-persist</span></span>](/cli/azure/config/param-persist) | <span data-ttu-id="9fe07-166">Lokale Gültigkeit für ein bestimmtes Arbeitsverzeichnis</span><span class="sxs-lookup"><span data-stu-id="9fe07-166">Scoped locally to a specific working directory</span></span> | <span data-ttu-id="9fe07-167">Automatische Festlegung nach Aktivierung von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="9fe07-167">Set automatically once persisted parameters are turned on</span></span> | <span data-ttu-id="9fe07-168">Verwendung für sequenzielle Befehle einzelner Workloads</span><span class="sxs-lookup"><span data-stu-id="9fe07-168">Use for individual workload sequential commands.</span></span>

### <a name="command-examples"></a><span data-ttu-id="9fe07-169">Befehlsbeispiele</span><span class="sxs-lookup"><span data-stu-id="9fe07-169">Command examples</span></span>

<span data-ttu-id="9fe07-170">Verwenden Sie `az config param-persist`, um eine globale Variable festzulegen, die bei der Erstellung eines Azure-Speicherkontos verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9fe07-170">Use `az config param-persist` to set a global variable used in the creation of an Azure storage account.</span></span>

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="9fe07-171">Die CLI-Befehlsausgabe zeigt, dass ein neues Speicherkonto in der Ressourcengruppe unter der globalen Variablen „myGlobalVariableRG“ erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9fe07-171">CLI command output shows that a new storage account was created in the resource group found in the global variable, \`myGlobalVariableRG'.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

<span data-ttu-id="9fe07-172">Verwenden Sie `az config param-persist`, um permanente Parameter festzulegen, die bei der Erstellung eines Azure-Speicherkontos verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="9fe07-172">Use `az config param-persist` to set persisted parameters used in the creation of an Azure storage account.</span></span>  <span data-ttu-id="9fe07-173">Wenn eine globale Variable für dasselbe Objekt festgelegt wird, wird die globale Variable durch den permanenten Parameter außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="9fe07-173">If a global variable is set for the same object, the persisted parameter will override the global variable.</span></span>

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="9fe07-174">Auch wenn eine globale Variable für die Ressourcengruppe mit dem Wert `myGlobalVariableRG` festgelegt ist und permanente Parameter aktiviert sind, wird das neue Speicherkonto mit `myParamPersistRG` erstellt.</span><span class="sxs-lookup"><span data-stu-id="9fe07-174">Even with a global variable set for resource group with a value of `myGlobalVariableRG`, with persisted parameters turned on, the new storage account was created with `myParamPersistRG`.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a><span data-ttu-id="9fe07-175">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9fe07-175">See also</span></span>

* [<span data-ttu-id="9fe07-176">Tutorial: Verwenden von permanenten Parametern mit sequenziellen Azure CLI-Befehlen</span><span class="sxs-lookup"><span data-stu-id="9fe07-176">Tutorial: Use persisted parameter with sequential Azure CLI commands</span></span>](param-persist-tutorial.md)
* [<span data-ttu-id="9fe07-177">Azure CLI-Konfiguration mit „az configure“</span><span class="sxs-lookup"><span data-stu-id="9fe07-177">Azure CLI Configuration using az configure</span></span>](azure-cli-configuration.md)

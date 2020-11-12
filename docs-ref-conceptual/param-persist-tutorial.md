---
title: 'Tutorial: Verwenden von permanenten Parametern mit der Azure CLI'
description: Tutorial zur Verwendung von „az config param-persist“ zum Speichern von Azure CLI-Parameterwerten für die wiederholte Nutzung
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 49bf1d852f000dfbe6251cc15bd63e780b3bc91a
ms.sourcegitcommit: 8d514f4147d6edfc02d8d95d5a4243d100a7fcc9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2020
ms.locfileid: "93423190"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a><span data-ttu-id="f09f5-103">Tutorial: Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen</span><span class="sxs-lookup"><span data-stu-id="f09f5-103">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>

<span data-ttu-id="f09f5-104">Die Azure CLI verfügt über eine Option für permanente Parameter, mit der Sie Parameterwerte für die Wiederverwendung speichern können.</span><span class="sxs-lookup"><span data-stu-id="f09f5-104">Azure CLI offers persisted parameters that enable you to store parameter values for continued use.</span></span>  <span data-ttu-id="f09f5-105">In diesem Tutorial wird beschrieben, wie Sie permanente Werte nutzen und diese lokalen Werte zum effizienten Ausführen von sequenziellen Befehlen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f09f5-105">In this tutorial, you learn how to work with persisted values, and use these local values to efficiently execute sequential commands.</span></span>

<span data-ttu-id="f09f5-106">In diesem Tutorial lernen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="f09f5-106">In this tutorial, you will learn to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="f09f5-107">Verwenden von **az config param-persist** -Referenzbefehlen</span><span class="sxs-lookup"><span data-stu-id="f09f5-107">Use **az config param-persist** reference commands</span></span>
> * <span data-ttu-id="f09f5-108">Ausführen von sequenziellen Befehlen mit permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-108">Execute sequential commands using persisted parameters</span></span>

<span data-ttu-id="f09f5-109">In diesem Tutorial werden die folgenden Azure CLI-Befehle verwendet:</span><span class="sxs-lookup"><span data-stu-id="f09f5-109">This tutorial uses the following Azure CLI commands</span></span>

- [<span data-ttu-id="f09f5-110">az config param-persist delete</span><span class="sxs-lookup"><span data-stu-id="f09f5-110">az config param-persist delete</span></span>](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [<span data-ttu-id="f09f5-111">az config param-persist off</span><span class="sxs-lookup"><span data-stu-id="f09f5-111">az config param-persist off</span></span>](/cli/azure/config/param-persist#az_config_param_persist_off)
- [<span data-ttu-id="f09f5-112">az config param-persist on</span><span class="sxs-lookup"><span data-stu-id="f09f5-112">az config param-persist on</span></span>](/cli/azure/config/param-persist#az_config_param_persist_on)
- [<span data-ttu-id="f09f5-113">az config param-persist show</span><span class="sxs-lookup"><span data-stu-id="f09f5-113">az config param-persist show</span></span>](/cli/azure/config/param-persist#az_config_param_persist_show)
- [<span data-ttu-id="f09f5-114">az function app create</span><span class="sxs-lookup"><span data-stu-id="f09f5-114">az function app create</span></span>](/cli/azure/functionapp#az_functionapp_create)
- [<span data-ttu-id="f09f5-115">az group create</span><span class="sxs-lookup"><span data-stu-id="f09f5-115">az group create</span></span>](/cli/azure/group#az_group_create)
- [<span data-ttu-id="f09f5-116">az storage account create</span><span class="sxs-lookup"><span data-stu-id="f09f5-116">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)


<span data-ttu-id="f09f5-117">Wenn Sie kein Azure-Abonnement besitzen, können Sie ein [kostenloses Konto](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) erstellen, bevor Sie beginnen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-117">If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) before you begin.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f09f5-118">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f09f5-118">Prerequisites</span></span>

1. [<span data-ttu-id="f09f5-119">Installieren der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="f09f5-119">Install the Azure CLI</span></span>](install-azure-cli.md)

   <span data-ttu-id="f09f5-120">Wenn Sie möchten, können Sie auch Azure Cloud Shell verwenden, um die Schritte in diesem Tutorial auszuführen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-120">If you prefer, you can also use Azure Cloud Shell to complete the steps in this tutorial.</span></span>  <span data-ttu-id="f09f5-121">Azure Cloud Shell ist eine interaktive Shellumgebung, die Sie über Ihren Browser nutzen können.</span><span class="sxs-lookup"><span data-stu-id="f09f5-121">Azure Cloud Shell is an interactive shell environment that you use through your browser.</span></span>  <span data-ttu-id="f09f5-122">Starten Sie Cloud Shell mit einer der folgenden Methoden:</span><span class="sxs-lookup"><span data-stu-id="f09f5-122">Start Cloud Shell by using one of these methods:</span></span>

   - <span data-ttu-id="f09f5-123">Öffnen Sie Cloud Shell, indem Sie zu [https://shell.azure.com](https://shell.azure.com) navigieren.</span><span class="sxs-lookup"><span data-stu-id="f09f5-123">Open Cloud Shell by going to [https://shell.azure.com](https://shell.azure.com)</span></span>

   - <span data-ttu-id="f09f5-124">Wählen Sie im [Azure-Portal](https://portal.azure.com) rechts oben im Menü die Schaltfläche **Cloud Shell** aus.</span><span class="sxs-lookup"><span data-stu-id="f09f5-124">Select the **Cloud Shell** button on the menu bar at the upper right corner in the [Azure portal](https://portal.azure.com)</span></span>

1. <span data-ttu-id="f09f5-125">Gehen Sie wie folgt vor, falls Sie eine lokale Installation der Azure CLI verwenden:</span><span class="sxs-lookup"><span data-stu-id="f09f5-125">If you are using a local install of the Azure CLI, complete the following:</span></span>
   - <span data-ttu-id="f09f5-126">Melden Sie sich mit dem Befehl [az login](/cli/azure/reference-index#az-login) an, und führen Sie anschließend die in Ihrem Terminal angezeigten Schritte für den Authentifizierungsprozess aus.</span><span class="sxs-lookup"><span data-stu-id="f09f5-126">Sign in using the [az login](/cli/azure/reference-index#az-login) command, then follow the steps displayed in your terminal to complete the authentication process.</span></span>

     ```azurecli
     az login
     ```
    - <span data-ttu-id="f09f5-127">Für dieses Tutorial ist mindestens Version 2.12.0 der Azure CLI erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f09f5-127">This tutorial requires version 2.12.0 or later of the Azure CLI.</span></span>  <span data-ttu-id="f09f5-128">Führen Sie [az version](/cli/azure/reference-index?#az_version) aus, um die installierte Version und die abhängigen Bibliotheken zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="f09f5-128">Run [az version](/cli/azure/reference-index?#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="f09f5-129">Führen Sie [az upgrade](/cli/azure/reference-index?#az_upgrade) aus, um das Upgrade auf die aktuelle Version durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-129">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index?#az_upgrade).</span></span>

## <a name="1-determine-your-local-directory"></a><span data-ttu-id="f09f5-130">1. Ermitteln Ihres lokalen Verzeichnisses</span><span class="sxs-lookup"><span data-stu-id="f09f5-130">1. Determine your local directory</span></span>

<span data-ttu-id="f09f5-131">Permanente Parameterwerte werden im Arbeitsverzeichnis des Azure-Speicherkontos gespeichert, das von Azure Cloud Shell verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f09f5-131">Persisted parameter values are stored in the working directory of the Azure storage account used by Azure Cloud Shell.</span></span>  <span data-ttu-id="f09f5-132">Bei Verwendung einer lokalen Installation der Azure CLI werden die Werte im Arbeitsverzeichnis auf Ihrem Computer gespeichert.</span><span class="sxs-lookup"><span data-stu-id="f09f5-132">If you are using a local install of the Azure CLI, values are stored in the working directory on your machine.</span></span>

<span data-ttu-id="f09f5-133">Nutzen Sie diese vertrauten CLI-Befehle, um das von der Azure CLI verwendete Arbeitsverzeichnis zu ermitteln, zu erstellen oder zu ändern.</span><span class="sxs-lookup"><span data-stu-id="f09f5-133">To find, create or change the working directory being used by the Azure CLI, use these familiar CLI commands.</span></span>

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a><span data-ttu-id="f09f5-134">2. Aktivieren von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-134">2. Turn on Persisted parameters</span></span>

<span data-ttu-id="f09f5-135">[Permanente Parameter](/cli/azure/param-persist) müssen aktiviert werden, bevor Parameterwerte gespeichert werden können.</span><span class="sxs-lookup"><span data-stu-id="f09f5-135">[Persisted parameters](/cli/azure/param-persist) must be turned on before parameter values can be stored.</span></span>  <span data-ttu-id="f09f5-136">Sie erhalten eine Warnung, solange sich **az config param-persist** noch in der Experimentierphase befindet.</span><span class="sxs-lookup"><span data-stu-id="f09f5-136">You will receive a warning until **az config param-persist** moves out of the experimental stage.</span></span>  <span data-ttu-id="f09f5-137">Unter [Übersicht: Azure CLI-Referenztypen und -Status](/cli/azure/reference-types-and-status) finden Sie Informationen zu den Referenztypen, dem Status und den Supportebenen der Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="f09f5-137">See [Overview: Azure CLI reference types and status](/cli/azure/reference-types-and-status) to learn about the Azure CLI reference types, status, and support levels.</span></span>

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a><span data-ttu-id="f09f5-138">3. Erstellen permanenter Parameter</span><span class="sxs-lookup"><span data-stu-id="f09f5-138">3. Create persisted parameters</span></span>

<span data-ttu-id="f09f5-139">Führen Sie zum Speichern von Werten für permanente Parameter einen Azure CLI-Befehl Ihrer Wahl aus, der die zu speichernden Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="f09f5-139">To store values for persisted parameters, execute an Azure CLI command of your choice that contains the parameters you want to store.</span></span>  <span data-ttu-id="f09f5-140">Erstellen Sie beispielsweise eine Ressourcengruppe. Die Parameter **--location** und **--name** werden bei diesem Vorgang dann für die zukünftige Verwendung gespeichert.</span><span class="sxs-lookup"><span data-stu-id="f09f5-140">For example, create a resource group and the **--location** and **--name** parameters are stored for future use.</span></span>

1. <span data-ttu-id="f09f5-141">Speichern Sie den Speicherort und den Ressourcengruppennamen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-141">Store the location and resource group name.</span></span>
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. <span data-ttu-id="f09f5-142">Erstellen Sie mit den neuen permanenten Parametern ein Speicherkonto.</span><span class="sxs-lookup"><span data-stu-id="f09f5-142">Using the new persisted parameters, create a storage account.</span></span>

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="f09f5-143">Erstellen Sie einen permanenten Parameter, ohne eine neue Ressource zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-143">Create a persisted parameter without creating a new resource.</span></span>

   <span data-ttu-id="f09f5-144">Falls Sie keine neue Azure-Ressource erstellen möchten, können Sie die Parameter **resource_group_name** und **location** speichern, indem Sie andere Befehle wie **show** oder **list** verwenden.</span><span class="sxs-lookup"><span data-stu-id="f09f5-144">If you do not want to create a new Azure resource, **resource_group_name** and **location** parameters can be stored by using non-create commands like **show** or **list**.</span></span>   <span data-ttu-id="f09f5-145">Eine vollständige Liste mit unterstützten Parametern und der Aktion, die zum Beibehalten von Werten durchgeführt werden muss, finden Sie unter [Permanente Azure CLI-Parameter](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).</span><span class="sxs-lookup"><span data-stu-id="f09f5-145">See [Azure CLI persisted parameters](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) for a full list of supported parameters,   and the action needed to retain values.</span></span>  <span data-ttu-id="f09f5-146">In diesem Beispiel werden mit dem Befehl [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) auch alle Parameterwerte entfernt.</span><span class="sxs-lookup"><span data-stu-id="f09f5-146">This example also removes all parameter values by using the [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) command.</span></span>

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the **resource_group_name** stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a><span data-ttu-id="f09f5-147">4. Ersetzen von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-147">4. Replace persisted parameters</span></span>

<span data-ttu-id="f09f5-148">Zum Ersetzen eines gespeicherten Parameterwerts müssen Sie einfach nur einen Befehl mit einem anderen Wert ausführen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-148">Replacing a stored parameter value is as simple as executing a command containing a different value.</span></span>

1. <span data-ttu-id="f09f5-149">Erstellen Sie neue permanente Parameter.</span><span class="sxs-lookup"><span data-stu-id="f09f5-149">Create new persisted parameters.</span></span>
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="f09f5-150">Ersetzen Sie die neu gespeicherten Werte.</span><span class="sxs-lookup"><span data-stu-id="f09f5-150">Replace the newly stored values.</span></span>

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > <span data-ttu-id="f09f5-151">Auch wenn die Option für permanente Parameter aktiviert ist, müssen Sie sie nicht unbedingt verwenden.</span><span class="sxs-lookup"><span data-stu-id="f09f5-151">Even if persisted parameters are turned on, you don't have to use them.</span></span>  <span data-ttu-id="f09f5-152">Sie können weiterhin Befehle mit allen angegebenen Parameterwerten ausführen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-152">You can still execute commands with all parameter values specified.</span></span>  <span data-ttu-id="f09f5-153">Hierbei sollten Sie aber beachten, dass Sie bei Aktivierung der Option für permanente Parameter _neue permanente Parameter erstellen bzw. vorhandene überschreiben._</span><span class="sxs-lookup"><span data-stu-id="f09f5-153">However, be aware that with persisted parameters turned on, _you will be creating new persisted parameters, or overwriting existing ones._</span></span>

## <a name="5-execute-sequential-commands"></a><span data-ttu-id="f09f5-154">5. Ausführen von sequenziellen Befehlen</span><span class="sxs-lookup"><span data-stu-id="f09f5-154">5. Execute sequential commands</span></span>

<span data-ttu-id="f09f5-155">Mit diesen Skripts wird eine Azure-Funktions-App mit einem Verbrauchsplan erstellt.</span><span class="sxs-lookup"><span data-stu-id="f09f5-155">These scripts create an Azure Function app using the Consumption plan.</span></span>

### <a name="using-persisted-parameters"></a>[<span data-ttu-id="f09f5-156">Verwenden von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-156">Using persisted parameters</span></span>](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[<span data-ttu-id="f09f5-157">Ohne permanente Parameter</span><span class="sxs-lookup"><span data-stu-id="f09f5-157">Without persisted parameters</span></span>](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a><span data-ttu-id="f09f5-158">6. Löschen von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-158">6. Delete persisted parameters</span></span>

<span data-ttu-id="f09f5-159">Verwenden Sie den Befehl [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete), um Einträge zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-159">Use the [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) command to remove entries.</span></span>

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete --name resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> <span data-ttu-id="f09f5-160">Permanente Parameter werden nicht aktualisiert, wenn eine Azure-Ressource gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="f09f5-160">Persisted parameters do not get updated when an Azure resource is deleted.</span></span>
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a><span data-ttu-id="f09f5-161">7. Deaktivieren von permanenten Parametern</span><span class="sxs-lookup"><span data-stu-id="f09f5-161">7. Turn persisted parameters off</span></span>

<span data-ttu-id="f09f5-162">Sie können permanente Parameter deaktivieren, indem Sie den Befehl [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) verwenden. Ihre gespeicherten Daten für permanente Parameter werden hierbei nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="f09f5-162">You can turn persisted parameters off by using the [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) command, but your saved persisted parameters data won't be deleted.</span></span>

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a><span data-ttu-id="f09f5-163">8. Bereinigen von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f09f5-163">8. Clean up resources</span></span>

<span data-ttu-id="f09f5-164">Wenn Sie die Ressourcen nicht mehr benötigen, führen Sie den Befehl [az group delete](/cli/azure/group) aus, um die Ressourcengruppe und alle zugehörigen Ressourcen zu löschen.</span><span class="sxs-lookup"><span data-stu-id="f09f5-164">When no longer needed, use the [az group delete](/cli/azure/group) command to remove the resource group, and all related resources.</span></span>

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a><span data-ttu-id="f09f5-165">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f09f5-165">See also</span></span>

- [<span data-ttu-id="f09f5-166">Permanente Azure CLI-Parameter</span><span class="sxs-lookup"><span data-stu-id="f09f5-166">(How to work with Azure CLI persisted parameters</span></span>](param-persist-howto.md)
- [<span data-ttu-id="f09f5-167">Azure CLI-Konfiguration mit „az configure“</span><span class="sxs-lookup"><span data-stu-id="f09f5-167">Azure CLI Configuration using az configure</span></span>](/cli/azure/azure-cli-configuration)

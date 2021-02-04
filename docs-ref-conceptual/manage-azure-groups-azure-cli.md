---
title: Verwalten von Azure-Ressourcengruppen mithilfe der Azure-Befehlszeilenschnittstelle
description: Hier erfahren Sie mehr über Azure-Ressourcengruppen und die Verwendung der Azure CLI zum Verwalten Ihrer Ressourcengruppen. Informieren Sie sich über dauerhaft gespeicherte und standardmäßige Ressourcengruppen.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496077"
---
# <a name="working-with-resource-groups-in-azure-cli"></a><span data-ttu-id="83c2f-104">Arbeiten mit Ressourcengruppen über die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="83c2f-104">Working with resource groups in Azure CLI</span></span>

<span data-ttu-id="83c2f-105">Eine Azure-Ressourcengruppe ist ein Container, der verwandte Ressourcen für eine Azure-Lösung enthält.</span><span class="sxs-lookup"><span data-stu-id="83c2f-105">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="83c2f-106">Eine Ressourcengruppe kann Speicher, virtuelle Computer, Apps, Dashboards, Dienste oder nahezu alle von Ihnen in Azure verwendeten Komponenten enthalten.</span><span class="sxs-lookup"><span data-stu-id="83c2f-106">A resource group might contain storage, virtual machines, apps, dashboards, services, or almost anything you deal with in Azure.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="83c2f-107">Erstellen einer Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="83c2f-107">Create a resource group</span></span>

<span data-ttu-id="83c2f-108">Verwenden Sie zum Erstellen einer Ressourcengruppe den Befehl [az group create](/cli/azure/group#az_group_create):</span><span class="sxs-lookup"><span data-stu-id="83c2f-108">To create a resource group, use the [az group create](/cli/azure/group#az_group_create) command:</span></span>

```azurecli
az group create --name MyResourceGroup --location eastus
```

<span data-ttu-id="83c2f-109">Eine Ressourcengruppe gehört jeweils nur zu einem Standort.</span><span class="sxs-lookup"><span data-stu-id="83c2f-109">A resource group belongs to a single location.</span></span> <span data-ttu-id="83c2f-110">Führen Sie zum Anzeigen aller im aktuellen Abonnement unterstützten Standorte den Befehl [az account list-locations](/cli/azure/account#az_account_list_locations) aus:</span><span class="sxs-lookup"><span data-stu-id="83c2f-110">To see all the locations supported in your current subscription, run the [az account list-locations](/cli/azure/account#az_account_list_locations) command:</span></span>

```azurecli
az account list-locations
```

<span data-ttu-id="83c2f-111">Verwenden Sie zum Anzeigen aller Ressourcengruppen für Ihr aktuelles Abonnement den Befehl [az group list](/cli/azure/group#az_group_list):</span><span class="sxs-lookup"><span data-stu-id="83c2f-111">To see all the resource groups for your current subscription, use the [az group list](/cli/azure/group#az_group_list) command:</span></span>

```azurecli
az group list --output table
```

> [!TIP]
> <span data-ttu-id="83c2f-112">Der Parameter `--output` ist ein globaler Parameter und für alle Befehle verfügbar.</span><span class="sxs-lookup"><span data-stu-id="83c2f-112">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="83c2f-113">Mit dem Wert **table** wird die Ausgabe in einem benutzerfreundlichen Format angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83c2f-113">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="83c2f-114">Weitere Informationen finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="83c2f-114">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="83c2f-115">Wenn Sie eine Ressource erstellen, müssen Sie sie in einer Ressourcengruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-115">When you create a resource, you create it in a resource group.</span></span> <span data-ttu-id="83c2f-116">Das folgende Beispiel zeigt ein mithilfe des Befehls [az storage account create](/cli/azure/storage/account#az_storage_account_create) erstelltes Speicherkonto:</span><span class="sxs-lookup"><span data-stu-id="83c2f-116">The following example shows a storage account created by using the [az storage account create](/cli/azure/storage/account#az_storage_account_create) command:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

<span data-ttu-id="83c2f-117">Führen Sie zum Entfernen einer Ressourcengruppe den Befehl [az group delete](/cli/azure/group#az_group_delete) aus.</span><span class="sxs-lookup"><span data-stu-id="83c2f-117">To remove a resource group, run the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
```

<span data-ttu-id="83c2f-118">Beim Entfernen einer Ressourcengruppe löschen Sie alle dazugehörigen Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-118">When you remove a resource group, you delete all the resources that belong to it.</span></span> <span data-ttu-id="83c2f-119">Es gibt keine Option, das Löschen von Ressourcen rückgängig zu machen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-119">There's no option to undelete resources.</span></span> <span data-ttu-id="83c2f-120">Wenn Sie einen der Befehle in diesem Artikel ausprobieren, wird beim Löschen der von Ihnen erstellten Ressourcengruppen Ihr Konto bereinigt.</span><span class="sxs-lookup"><span data-stu-id="83c2f-120">If you try any of the commands in this article, deleting the resource groups you create cleans up your account.</span></span>

## <a name="persist-a-resource-group"></a><span data-ttu-id="83c2f-121">Dauerhaftes Speichern einer Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="83c2f-121">Persist a resource group</span></span>

<span data-ttu-id="83c2f-122">Die Parameterpersistenz ermöglicht die Wiederverwendung von Werten für bestimmte Parameter, einschließlich Ressourcengruppen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-122">Parameter persistence allows you to reuse values for certain parameters, including resource groups.</span></span>

<span data-ttu-id="83c2f-123">Aktivieren Sie zunächst das Persistenzfeature mithilfe des Befehls [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):</span><span class="sxs-lookup"><span data-stu-id="83c2f-123">First, turn on the persistence feature by using the [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) command:</span></span>

```azurecli
az config param-persist on
```

<span data-ttu-id="83c2f-124">Erstellen Sie nach dem Aktivieren der Persistenz eine weitere Ressourcengruppe:</span><span class="sxs-lookup"><span data-stu-id="83c2f-124">After turning on persistence, create another resource group:</span></span>

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

<span data-ttu-id="83c2f-125">Solange Persistenz aktiviert ist, können Sie den Parameter `--resource-group` in künftigen Befehlen auslassen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-125">As long as persistence is on, your can leave the `--resource-group` parameter out of future commands.</span></span> <span data-ttu-id="83c2f-126">Der folgende Befehl erstellt ein Speicherkonto in der Gruppe **OtherResourceGroup**.</span><span class="sxs-lookup"><span data-stu-id="83c2f-126">The following command creates a storage account in the **OtherResourceGroup** group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="83c2f-127">Wenn Sie eine Ressourcengruppe im Befehl angeben, hat dies Vorrang.</span><span class="sxs-lookup"><span data-stu-id="83c2f-127">If you specify a resource group in the command, that takes precedence.</span></span> <span data-ttu-id="83c2f-128">Mit dem folgenden Befehl wird eine Speichergruppe in einer Ressourcengruppe namens **StorageGroups** erstellt:</span><span class="sxs-lookup"><span data-stu-id="83c2f-128">The following command creates a storage group in a resource group called **StorageGroups**:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

<span data-ttu-id="83c2f-129">Wenn Sie jedoch eine andere Ressourcengruppe als Wert angeben, setzt die Azure CLI den dauerhaft gespeicherten Wert zurück.</span><span class="sxs-lookup"><span data-stu-id="83c2f-129">Once you specify another resource group as a value, however, Azure CLI resets the persisted value.</span></span> <span data-ttu-id="83c2f-130">Neue Befehle verwenden **StorageGroups** als Ressourcengruppe.</span><span class="sxs-lookup"><span data-stu-id="83c2f-130">New commands use **StorageGroups** as the resource group.</span></span> <span data-ttu-id="83c2f-131">Die dauerhaft gespeicherten Werte können mit dem Befehl [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="83c2f-131">You can see the persisted values by using the [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) command:</span></span>

```azurecli
az config param-persist show
```

<span data-ttu-id="83c2f-132">Mit diesem Befehl werden die aktuellen dauerhaft gespeicherten Werte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83c2f-132">This command shows you the current persisted values.</span></span> <span data-ttu-id="83c2f-133">Diese Werte werden in einer Datei namens *local_context_\<username>* in dem ausgeblendeten Verzeichnis *.azure* gespeichert.</span><span class="sxs-lookup"><span data-stu-id="83c2f-133">These values are stored in a file called *local_context_\<username>* in a hidden directory called *.azure*.</span></span> <span data-ttu-id="83c2f-134">Die Azure CLI erstellt das Verzeichnis am aktuellen Standort, wenn Sie zum ersten Mal einen persistenten Wert erstellen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-134">Azure CLI creates the directory in your current location when you first create a persistent value.</span></span>

<span data-ttu-id="83c2f-135">Wenn Sie keine dauerhaft gespeicherten Parameter mehr verwenden möchten, führen Sie den Befehl [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) aus:</span><span class="sxs-lookup"><span data-stu-id="83c2f-135">When you're done using persisted parameters, run the [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) command:</span></span>

```azurecli
az config param-persist off
```

<span data-ttu-id="83c2f-136">Von der Azure CLI werden die dauerhaft gespeicherten Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="83c2f-136">Azure CLI saves your persisted values.</span></span> <span data-ttu-id="83c2f-137">Diese können in der lokalen Kontextdatei angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="83c2f-137">You can see them in the local context file.</span></span> <span data-ttu-id="83c2f-138">Wenn Sie die Parameterpersistenz erneut aktivieren, sind diese Werte bereits festgelegt.</span><span class="sxs-lookup"><span data-stu-id="83c2f-138">If you turn on parameter persistence again, those values are already set.</span></span>

<span data-ttu-id="83c2f-139">Weitere Informationen zur Verwendung der Befehle vom Typ [az config param-persist](/cli/azure/config/param-persist) finden Sie unter [Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen](/cli/azure/param-persist-tutorial).</span><span class="sxs-lookup"><span data-stu-id="83c2f-139">For more information about using the [az config param-persist](/cli/azure/config/param-persist) commands, see [Use persisted parameters to simplify sequential Azure CLI commands](/cli/azure/param-persist-tutorial).</span></span>

## <a name="set-a-default-resource-group"></a><span data-ttu-id="83c2f-140">Festlegen einer Standardressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="83c2f-140">Set a default resource group</span></span>

<span data-ttu-id="83c2f-141">Sie können eine Standardressourcengruppe für alle Befehle festlegen, die Sie über die lokale Azure CLI oder über Azure Cloud Shell ausführen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-141">You can set a default resource group for all the commands that you run from your local Azure CLI or from Azure Cloud Shell.</span></span> <span data-ttu-id="83c2f-142">Die Azure CLI speichert diese Konfiguration lokal in einer Datei vom Typ *config*.</span><span class="sxs-lookup"><span data-stu-id="83c2f-142">Azure CLI stores this configuration locally in a *config* file.</span></span> <span data-ttu-id="83c2f-143">Führen Sie zum Anzeigen der aktuellen Konfiguration den Befehl [az config get](/cli/azure/config#az_config_get) aus:</span><span class="sxs-lookup"><span data-stu-id="83c2f-143">To see your current configuration, run the [az config get](/cli/azure/config#az_config_get) command:</span></span>

```azurecli
az config get
```

<span data-ttu-id="83c2f-144">Im Ergebnis werden Standardressourcengruppen und andere Standardwerte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83c2f-144">The result shows default resource groups and other default values.</span></span> <span data-ttu-id="83c2f-145">Wenn Sie die Azure CLI zum ersten Mal verwenden, sind die Ergebnisse möglicherweise leer.</span><span class="sxs-lookup"><span data-stu-id="83c2f-145">If you're using Azure CLI for the first time, the results might be empty.</span></span>

<span data-ttu-id="83c2f-146">Führen Sie zum Festlegen einer Standardressourcengruppe für Ihre Azure CLI-Installation den Befehl [az config set](/cli/azure/config#az_config_set) aus:</span><span class="sxs-lookup"><span data-stu-id="83c2f-146">To set a default resource group for your Azure CLI installation, run the [az config set](/cli/azure/config#az_config_set) command:</span></span>

```azurecli
az config set defaults.group=MyResourceGroup
```

<span data-ttu-id="83c2f-147">Mit dem Befehl wird ein Wert für einen angegebenen Schlüssel festgelegt, in diesem Fall `defaults.group`.</span><span class="sxs-lookup"><span data-stu-id="83c2f-147">The command sets a value for a specified key, in this case `defaults.group`.</span></span> <span data-ttu-id="83c2f-148">Informationen zu verfügbaren Konfigurationsoptionen finden Sie unter [Azure CLI-Konfiguration](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="83c2f-148">For available configuration options, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

> [!NOTE]
> <span data-ttu-id="83c2f-149">Mit dem Befehl [az config set](/cli/azure/config#az_config_set) wird nicht überprüft, ob die von Ihnen eingegebene Ressourcengruppe vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="83c2f-149">The [az config set](/cli/azure/config#az_config_set) command does not validate the existence of the resource group you enter.</span></span> <span data-ttu-id="83c2f-150">Mit dem Befehl wird lediglich das Schlüssel-Wert-Paar gespeichert.</span><span class="sxs-lookup"><span data-stu-id="83c2f-150">The command simply stores the key-value pair.</span></span>

<span data-ttu-id="83c2f-151">Nach dem Ausführen des Befehls erhalten Sie mit den folgenden beiden Befehlen dasselbe Ergebnis:</span><span class="sxs-lookup"><span data-stu-id="83c2f-151">After you run the command, the following two commands would give you the same result:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

<span data-ttu-id="83c2f-152">Eine Ressourcengruppe gehört zu einem Abonnement.</span><span class="sxs-lookup"><span data-stu-id="83c2f-152">A resource group belongs to a subscription.</span></span> <span data-ttu-id="83c2f-153">Wenn Ihre Organisation über mehrere Abonnements verfügt, müssen Sie das entsprechende Abonnement festlegen, bevor Sie eine Ressourcengruppe im Abonnement verwenden.</span><span class="sxs-lookup"><span data-stu-id="83c2f-153">If your organization has more than one subscription, you need to set that subscription before working with a resource group in the subscription.</span></span> <span data-ttu-id="83c2f-154">Gehört der Standardwert einer Ressourcengruppe nicht zu Ihrem aktuellen Abonnement, führt dies zu einem Fehler.</span><span class="sxs-lookup"><span data-stu-id="83c2f-154">If the default value of a resource group does not belong to your current subscription, an error results.</span></span> <span data-ttu-id="83c2f-155">Weitere Informationen zu mehreren Abonnements finden Sie unter [Verwenden mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="83c2f-155">For more information about multiple subscriptions, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="83c2f-156">Sie müssen den Standardwert nicht zurücksetzen, um andere Ressourcengruppen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="83c2f-156">You don't have to reset the default to use other resource groups.</span></span> <span data-ttu-id="83c2f-157">Geben Sie stattdessen die Ressourcengruppe an:</span><span class="sxs-lookup"><span data-stu-id="83c2f-157">Instead, specify the resource group:</span></span>

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

<span data-ttu-id="83c2f-158">Der Standardwert gilt nur für Sie.</span><span class="sxs-lookup"><span data-stu-id="83c2f-158">The default value is for you only.</span></span> <span data-ttu-id="83c2f-159">Er wirkt sich nicht auf andere Benutzer oder auf Änderungen aus, die Sie über das Azure-Portal vornehmen.</span><span class="sxs-lookup"><span data-stu-id="83c2f-159">It won't affect other users or changes you make through the Azure portal.</span></span>

<span data-ttu-id="83c2f-160">Wenn Sie dauerhaft gespeicherte Parameterwerte wie in diesem Artikel beschrieben verwenden, haben diese Werte Vorrang vor den in der Datei *config* festgelegten Standardwerten.</span><span class="sxs-lookup"><span data-stu-id="83c2f-160">If you are using persisted parameter values, as described in this article, those values take precedence over defaults set in the *config* file.</span></span>

## <a name="clean-up-resources"></a><span data-ttu-id="83c2f-161">Bereinigen von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="83c2f-161">Clean up resources</span></span>

<span data-ttu-id="83c2f-162">Wenn Sie einen der Befehle in diesem Artikel ausprobiert haben, können Sie alle erstellten Ressourcen mithilfe des Befehls [az group delete](/cli/azure/group#az_group_delete) entfernen:</span><span class="sxs-lookup"><span data-stu-id="83c2f-162">If you tried any of the commands in this article, you can remove any resources you created by using the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

<span data-ttu-id="83c2f-163">Mit diesem Befehl werden die Gruppe und gleichzeitig alle darin enthaltenen Ressourcen gelöscht.</span><span class="sxs-lookup"><span data-stu-id="83c2f-163">This command removes the group and all the resources that it contains at once.</span></span>

<span data-ttu-id="83c2f-164">Sie können die persistenten Parameter mithilfe des Befehls [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) entfernen:</span><span class="sxs-lookup"><span data-stu-id="83c2f-164">You can remove the persistent parameters by running the [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) command:</span></span>

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a><span data-ttu-id="83c2f-165">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="83c2f-165">See also</span></span>

[<span data-ttu-id="83c2f-166">Azure CLI-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="83c2f-166">Azure CLI configuration</span></span>](/cli/azure/azure-cli-configuration)

[<span data-ttu-id="83c2f-167">Tutorial: Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen</span><span class="sxs-lookup"><span data-stu-id="83c2f-167">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>](/cli/azure/param-persist-tutorial)

[<span data-ttu-id="83c2f-168">Verwenden mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="83c2f-168">Use multiple Azure subscriptions</span></span>](manage-azure-subscriptions-azure-cli.md)

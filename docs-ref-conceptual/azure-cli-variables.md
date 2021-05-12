---
title: Angeben von Werten in Azure CLI-Befehlen
description: Erfahren Sie, wie Sie Werte (einschließlich Variablen) an Azure CLI-Befehle übergeben und allgemeine Werte wiederverwenden können.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-cli
ms.topic: how-to
ms.date: 03/01/2021
ms.custom: template-how-to, devx-track-azurecli
ms.openlocfilehash: 4c8f9a4146e7343376eff670eabb1cdb89f4e204
ms.sourcegitcommit: bff138c7d3cd3ce8c90c5809b0e812be71959504
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/14/2021
ms.locfileid: "107385806"
---
# <a name="specifying-values-in-azure-cli-commands"></a>Angeben von Werten in Azure CLI-Befehlen

Neben dem direkten Angeben von Werten in einem Befehl können Sie Werte auf verschiedene Weise bereitstellen:

* Verwenden von Shellvariablen
* Festlegen eines Abonnements für die Verwendung in mehreren Befehlen
* Erstellen von Standardwerten für einige Parameter
* Verwenden von permanenten Werten für einige Parameter

In diesem Artikel werden verschiedene Möglichkeiten zum Angeben von Werten in Azure CLI Befehlen erläutert.

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="use-shell-variables"></a>Verwenden von Shellvariablen

Die Azure CLI wird in einer Shell ausgeführt. In diesem Artikel wird Bash verwendet. Weitere Informationen zu anderen Shells finden Sie unter [Effektive Verwendung der Azure CLI](/cli/azure/use-cli-effectively). In Bash können Sie mithilfe von Variablen Parametermeter an Befehle übergeben. Durch die Verwendung von Variablen können außerdem Befehle (schrittweise oder in Skripts) wiederverwendet werden.

In diesem Beispiel wird ein neuer Speicherdatenträger vom selben Typ wie der Speicherdatenträger auf einem vorhandenen virtuellen Computer erstellt.

```azurecli
# Assign values to variables
MyResourceGroup=ContosoRGforVM
MySubscription="Contoso subscription"
vmName=VM01

# Get a value for a variable based on an existing virtual machine
osType=$(az vm get-instance-view --resource-group $MyResourceGroup \
   --name $vmName --subscription "$MySubscription" \
   --query 'storageProfile.osDisk.osType' --output tsv)

# Create a disk of the same type by using the variable value
az disk create --resource-group $MyResourceGroup --name DestinationDisk --size-gb 20 --os-type $osType
```

In diesem Beispiel werden Variablen Werte zugewiesen, die wiederverwendet werden (z. B. **MyResourceGroup**). Mit einem Befehl wird ein Wert abgerufen, der **osType** zugewiesen werden soll.

Wenn Sie einer Variablen einen Wert aus einem anderen Befehl zuweisen, müssen Sie sicherstellen, dass der Befehl ein kompatibles Ausgabeformat verwendet. Der Befehl [az vm get-instance-view](/cli/azure/vm#az_vm_get_instance_view) verwendet das Ausgabeformat `tsv`. Mit dieser Option werden die Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurückgegeben. Einige Ausgabeformate enthalten Struktur oder Zeichen wie Anführungszeichen. Weitere Informationen finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).

In diesem Beispiel muss die Variable **MySubscription** in Anführungszeichen stehen. Der zugehörige Wert enthält Leerzeichen, die vom Befehl nicht analysiert werden können. Wenn Sie nur mit Abonnement-IDs arbeiten, brauchen Sie keine Anführungszeichen zu verwenden.

## <a name="set-a-subscription"></a>Festlegen eines Abonnements

Für viele Befehle ist ein bestimmtes Abonnement erforderlich. Azure-Ressourcen befinden sich in Ressourcengruppen, die zu Abonnements gehören. Azure CLI verwendet ein Standardabonnement, wenn Sie sich in einer Sitzung befinden. Führen Sie den Befehl [az account show](/cli/azure/account#az_account_show) aus, um den aktuellen Abonnementwert anzuzeigen:

```azurecli
az account show --output table
```

Wahrscheinlich haben Sie nur Zugriff auf ein Abonnement. Weitere Informationen finden Sie unter [Verwenden von Azure-Abonnements mit Azure CLI](/cli/azure/manage-azure-subscriptions-azure-cli). Mit dem Befehl [az account set](/cli/azure/account#az_account_set) können Sie Ihr aktuelles Abonnement festlegen:

```azurecli
az account set --subscription "My Demos"
```

Nachdem Sie Ihr Abonnement festgelegt haben, können Sie auf den Parameter `--Subscription` verzichten. Weitere Informationen finden Sie unter [Verwenden mehrerer Azure-Abonnements mit Azure CLI](manage-azure-subscriptions-azure-cli.md).

## <a name="create-default-values"></a>Erstellen von Standardwerten

Mit dem Befehl [az config set](/cli/azure/config#az_config_set) können Sie Werte für einige Parameter festlegen. In diesem Beispiel wird eine Standardressourcengruppe festgelegt:

```azurecli
az config set defaults.group=ContosoRGforVM
```

Nachdem Sie diesen Befehl ausgeführt haben, können Sie mit dem folgenden Befehl ein Speicherkonto in der Ressourcengruppe „ContosoRGforVM“ erstellen:

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Beachten Sie, dass im Befehl keine Ressourcengruppe angegeben ist. Weitere Informationen finden Sie unter [Festlegen einer Standardressourcengruppe](manage-azure-groups-azure-cli.md#set-a-default-resource-group).

> [!TIP]
> Befehle, die Werte für Parameter auf unterschiedliche Weise abrufen, können verwirrend sein. Wenn ein Befehl ein unerwartetes Ergebnis liefert (z. B., dass eine Ressourcengruppe nicht gefunden werden kann), gibt es möglicherweise einen Standardwert.
>
> Wenn ein Fehler auftritt, führen Sie den Befehl erneut mit Angabe von Parameter und Wert aus. Ein expliziter Wert für einen Parameter hat immer Vorrang vor anderen Optionen.

Sie können auf diese Weise Werte für mehrere Parameter angeben. Weitere Informationen finden Sie unter [Azure CLI-Konfiguration](azure-cli-configuration.md).

## <a name="use-persistent-values"></a>Verwenden von permanenten Werten

Bei permanenten Parameterwerten können Sie einen Wert nur einmal angeben. Wenn Sie mehrere verwandte Aktionen in einer Ressourcengruppe ausführen, brauchen Sie diese Gruppe nicht wiederholt anzugeben.

Führen Sie diesen Befehl aus, um einen Parameterwert als permanent festzulegen:

```azurecli
az config param-persist on
```

Erstellen Sie nach dem Aktivieren der Permanenz eine Ressourcengruppe:

 ```azurecli
az group create --name ContosoStorageRG --location eastus
```

Solange Persistenz aktiviert ist, können Sie den Parameter `--resource-group` in künftigen Befehlen auslassen. Mit dem folgenden Befehl wird in der Gruppe „ContosoStorageRG“ ein Speicherkonto erstellt:

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Weitere Informationen finden Sie unter [Permanente Azure CLI-Parameter](/cli/azure/param-persist-howto).

## <a name="clean-up-resources"></a>Bereinigen von Ressourcen

Wenn Sie zum Ausprobieren eines Befehls in diesem Artikel Ressourcen erstellt haben, können Sie sie mit dem Befehl [az group delete](/cli/azure/group#az_group_delete) wieder entfernen:

```azurecli
az group delete --name ContosoRGforVM
az group delete --name ContosoStorageRG
```

Mit diesem Befehl werden die Gruppe und gleichzeitig alle darin enthaltenen Ressourcen gelöscht.

Sie können die permanenten Parameter mithilfe des Befehls [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) entfernen:

```azurecli
az config param-persist delete --all
```

## <a name="next-steps"></a>Nächste Schritte

* [Permanente Azure CLI-Parameter](param-persist-howto.md)
* [Arbeiten mit Ressourcengruppen über die Azure CLI](manage-azure-groups-azure-cli.md)
* [Erstellen einer Azure-Supportanfrage über die Azure CLI](azure-cli-support-request.md)

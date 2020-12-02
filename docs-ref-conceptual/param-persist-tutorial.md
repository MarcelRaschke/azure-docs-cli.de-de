---
title: 'Tutorial: Verwenden von permanenten Parametern mit der Azure CLI'
description: Tutorial zur Verwendung von „az config param-persist“ zum Speichern von Azure CLI-Parameterwerten für die wiederholte Nutzung
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 11/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 9db3035c9a50a2a3cc356f3fd7a49ab4f28652ee
ms.sourcegitcommit: 05b58a872cdd165805df62614000637144d80066
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96470433"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a>Tutorial: Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen

Die Azure CLI verfügt über eine Option für permanente Parameter, mit der Sie Parameterwerte für die Wiederverwendung speichern können.  In diesem Tutorial wird beschrieben, wie Sie permanente Werte nutzen und diese lokalen Werte zum effizienten Ausführen von sequenziellen Befehlen verwenden.

In diesem Tutorial lernen Sie Folgendes:

> [!div class="checklist"]
> * Verwenden von **az config param-persist**-Referenzbefehlen
> * Ausführen von sequenziellen Befehlen mit permanenten Parametern

In diesem Tutorial werden die folgenden Azure CLI-Befehle verwendet:

- [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off)
- [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on)
- [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show)
- [az function app create](/cli/azure/functionapp#az_functionapp_create)
- [az group create](/cli/azure/group#az_group_create)
- [az storage account create](/cli/azure/storage/account#az_storage_account_create)


Wenn Sie kein Azure-Abonnement besitzen, können Sie ein [kostenloses Konto](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) erstellen, bevor Sie beginnen.

## <a name="prerequisites"></a>Voraussetzungen

1. [Installieren der Azure-Befehlszeilenschnittstelle](install-azure-cli.md)

   Wenn Sie möchten, können Sie auch Azure Cloud Shell verwenden, um die Schritte in diesem Tutorial auszuführen.  Azure Cloud Shell ist eine interaktive Shellumgebung, die Sie über Ihren Browser nutzen können.  Starten Sie Cloud Shell mit einer der folgenden Methoden:

   - Öffnen Sie Cloud Shell, indem Sie zu [https://shell.azure.com](https://shell.azure.com) navigieren.

   - Wählen Sie im [Azure-Portal](https://portal.azure.com) rechts oben im Menü die Schaltfläche **Cloud Shell** aus.

1. Gehen Sie wie folgt vor, falls Sie eine lokale Installation der Azure CLI verwenden:
   - Melden Sie sich mit dem Befehl [az login](/cli/azure/reference-index#az-login) an, und führen Sie anschließend die in Ihrem Terminal angezeigten Schritte für den Authentifizierungsprozess aus.

     ```azurecli
     az login
     ```
    - Für dieses Tutorial ist mindestens Version 2.12.0 der Azure CLI erforderlich.  Führen Sie [az version](/cli/azure/reference-index?#az_version) aus, um die installierte Version und die abhängigen Bibliotheken zu ermitteln. Führen Sie [az upgrade](/cli/azure/reference-index?#az_upgrade) aus, um das Upgrade auf die aktuelle Version durchzuführen.

## <a name="1-determine-your-local-directory"></a>1. Ermitteln Ihres lokalen Verzeichnisses

Permanente Parameterwerte werden im Arbeitsverzeichnis des Azure-Speicherkontos gespeichert, das von Azure Cloud Shell verwendet wird.  Bei Verwendung einer lokalen Installation der Azure CLI werden die Werte im Arbeitsverzeichnis auf Ihrem Computer gespeichert.

Nutzen Sie diese vertrauten CLI-Befehle, um das von der Azure CLI verwendete Arbeitsverzeichnis zu ermitteln, zu erstellen oder zu ändern.

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a>2. Aktivieren von permanenten Parametern

[Permanente Parameter](/cli/azure/param-persist) müssen aktiviert werden, bevor Parameterwerte gespeichert werden können.  Sie erhalten eine Warnung, solange sich **az config param-persist** noch in der Experimentierphase befindet.  Unter [Übersicht: Azure CLI-Referenztypen und -Status](/cli/azure/reference-types-and-status) finden Sie Informationen zu den Referenztypen, dem Status und den Supportebenen der Azure CLI.

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a>3. Erstellen permanenter Parameter

Führen Sie zum Speichern von Werten für permanente Parameter einen Azure CLI-Befehl Ihrer Wahl aus, der die zu speichernden Parameter enthält.  Erstellen Sie beispielsweise eine Ressourcengruppe. Die Parameter **--location** und **--name** werden bei diesem Vorgang dann für die zukünftige Verwendung gespeichert.

1. Speichern Sie den Speicherort und den Ressourcengruppennamen.
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

1. Erstellen Sie mit den neuen permanenten Parametern ein Speicherkonto.

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

1. Erstellen Sie einen permanenten Parameter, ohne eine neue Ressource zu erstellen.

   Falls Sie keine neue Azure-Ressource erstellen möchten, können Sie die Parameter **resource_group_name** und **location** speichern, indem Sie andere Befehle wie **show** oder **list** verwenden.   Eine vollständige Liste mit unterstützten Parametern und der Aktion, die zum Beibehalten von Werten durchgeführt werden muss, finden Sie unter [Permanente Azure CLI-Parameter](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).  In diesem Beispiel werden mit dem Befehl [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) auch alle Parameterwerte entfernt.

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

## <a name="4-replace-persisted-parameters"></a>4. Ersetzen von permanenten Parametern

Zum Ersetzen eines gespeicherten Parameterwerts müssen Sie einfach nur einen Befehl mit einem anderen Wert ausführen.

1. Erstellen Sie neue permanente Parameter.
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

1. Ersetzen Sie die neu gespeicherten Werte.

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
   > Auch wenn die Option für permanente Parameter aktiviert ist, müssen Sie sie nicht unbedingt verwenden.  Sie können weiterhin Befehle mit allen angegebenen Parameterwerten ausführen.  Hierbei sollten Sie aber beachten, dass Sie bei Aktivierung der Option für permanente Parameter _neue permanente Parameter erstellen bzw. vorhandene überschreiben._

## <a name="5-execute-sequential-commands"></a>5. Ausführen von sequenziellen Befehlen

Mit diesen Skripts wird eine Azure-Funktions-App mit einem Verbrauchsplan erstellt.

### <a name="using-persisted-parameters"></a>[Verwenden von permanenten Parametern](#tab/azure-cli)

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

### <a name="without-persisted-parameters"></a>[Ohne permanente Parameter](#tab/azure-portal)

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

## <a name="6-delete-persisted-parameters"></a>6. Löschen von permanenten Parametern

Verwenden Sie den Befehl [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete), um Einträge zu entfernen.

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> Permanente Parameter werden nicht aktualisiert, wenn eine Azure-Ressource gelöscht wird.
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

## <a name="7-turn-persisted-parameters-off"></a>7. Deaktivieren von permanenten Parametern

Sie können permanente Parameter deaktivieren, indem Sie den Befehl [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) verwenden. Ihre gespeicherten Daten für permanente Parameter werden hierbei nicht gelöscht.

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a>8. Bereinigen von Ressourcen

Wenn Sie die Ressourcen nicht mehr benötigen, führen Sie den Befehl [az group delete](/cli/azure/group) aus, um die Ressourcengruppe und alle zugehörigen Ressourcen zu löschen.

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a>Siehe auch

- [Permanente Azure CLI-Parameter](param-persist-howto.md)
- [Azure CLI-Konfiguration mit „az configure“](/cli/azure/azure-cli-configuration)

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
# <a name="azure-cli-persisted-parameter"></a>Permanente Azure CLI-Parameter

Mit dem Azure CLI-Referenzbefehl [az config param-persist](/cli/azure/param-persist) können lokale permanente Parameterwerte für Azure CLI-Befehle festgelegt werden.  Es ist dann nicht mehr erforderlich, häufig verwendete Parameter ständig neu einzugeben. Beispielsweise sind die Parameter für den Speicherort (location) und die Ressourcengruppe (resource-group) in vielen CLI-Befehlen erforderlich, aber sie tragen nicht zur _Absicht_ des Befehls bei.  Wenn Sie Parameterwerte mit permanenten Parametern speichern, verringern Sie die Redundanz und können die CLI-Befehlssyntax deutlich verkürzen.

Von der CLI verwendete Konfigurationswerte werden in der folgenden Reihenfolge ausgewertet. Die Liste ist nach absteigender Priorität sortiert.

1. Befehlszeilenparameter
1. Werte im lokalen Arbeitsverzeichnis, die mit `az config param-persist` festgelegt werden
1. Umgebungsvariablen
1. In der Konfigurationsdatei enthaltene oder mit `az config` festgelegte Werte

[Installieren Sie die Azure CLI](install-azure-cli.md), oder öffnen Sie [Azure Cloud Shell](https://shell.azure.com), um die Skripts in diesem Artikel auszuführen.  Wenn Sie eine lokale Installation der Azure CLI verwenden, benötigen Sie für `az config param-persist`-Befehle Version 2.12.0 oder höher.  Führen Sie [az version](/cli/azure/reference-index#az_version) aus, um die installierte Version und die abhängigen Bibliotheken zu ermitteln. Führen Sie [az upgrade](/cli/azure/reference-index#az_upgrade) aus, um das Upgrade auf die aktuelle Version durchzuführen.  Azure Cloud Shell verfügt immer über die neueste Version der Azure CLI.

## <a name="persisted-parameter-data-file"></a>Datendatei für permanente Parameter

Permanente Parameterwerte sind in einer Datei mit dem Namen `.param_persist` enthalten, die in Ihrem Arbeitsverzeichnis gespeichert ist.  Bei Verwendung von [Azure Cloud Shell](https://shell.azure.com) zum Ausführen von Azure CLI-Befehlen befindet sich Ihr Arbeitsverzeichnis unter dem Speicherkonto, das von der Azure CLI verwendet wird.  Wenn Sie eine [lokale Installation](/install-azure-cli) der Azure CLI verwenden, befindet sich Ihr Arbeitsverzeichnis auf Ihrem lokalen Computer.  An beiden Speicherorten ist die Datei `.param_persist` ausgeblendet und sollte nicht manuell aktualisiert werden.

## <a name="persisted-parameter-storage-and-support"></a>Speicherung und Unterstützung von permanenten Parametern

Die folgenden Azure CLI-Parameter werden als permanente Parameter unterstützt.  Die Parameter `resource_group_name` und `location` werden auf andere Weise gespeichert, damit Sie sie als permanente Parameter festlegen können, _ohne_ einen Erstellungsbefehl auszuführen.

| Permanente Parameter | Speicheraktion | Unterstützt von
|-|-|-|
| location | Ausführung eines beliebigen Befehls | Alle Azure CLI-Referenzbefehle
| resource_group_name | Ausführung eines beliebigen Befehls | Alle Azure CLI-Referenzbefehle
| vnet_name | Ausführung eines Erstellungsbefehls | Nur Azure-Web-Apps
| storage_account_name | Ausführung eines Erstellungsbefehls |  Nur Azure-Web-Apps
| webapp_name | Ausführung eines Erstellungsbefehls | Nur Azure-Web-Apps
| function_app_name | Ausführung eines Erstellungsbefehls | Nur Azure Functions

## <a name="sample-script-using-persisted-parameters"></a>Beispielskript mit permanenten Parametern

Ohne permanente Parameter müssen für sequenzielle CLI-Befehle die gleichen Parameterwerte immer wieder angegeben werden.  Bei aktivierten permanenten Parametern können Ihre gespeicherten Parameterwerte in sequenziellen Befehlen weggelassen werden.  In diesem Beispiel werden der `location`, der `resource group name` oder der `storage account name` in den nachfolgenden Befehlen wiederholt.

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

## <a name="persisted-parameter-and-global-variable-comparison"></a>Vergleich zwischen permanenten Parametern und globalen Variablen

Es gibt zwei Azure CLI-Befehle, die als Standardparameterwerte verwendet werden können: `az configure` und `az config param-persist`.  Verwenden Sie den Befehl `az configure`, um _globale Variablen_ anzugeben, z. B. Gruppe, Speicherort oder Web.  Verwenden Sie `az param-persist`, um _lokale Standardwerte_ anzugeben, die für Ihre Workload eindeutig sind.  Gespeicherte Werte werden von der CLI anstelle von erforderlichen Argumenten verwendet.

> [!Important]
> Globale Kontextwerte werden durch permanente Parameter außer Kraft gesetzt.
>

| Verweis | `Scope` | Set | Zweck
|-|-|-|-|
[az configure](/cli/azure/reference-index#az_configure) | Globale Gültigkeit für die gesamte CLI | Explizite Festlegung mit `az configure --defaults` | Verwendung für Einstellungen, z. B. Protokollierung, Datensammlung und Standardargumentwerte
[az config param-persist](/cli/azure/config/param-persist) | Lokale Gültigkeit für ein bestimmtes Arbeitsverzeichnis | Automatische Festlegung nach Aktivierung von permanenten Parametern | Verwendung für sequenzielle Befehle einzelner Workloads

### <a name="command-examples"></a>Befehlsbeispiele

Verwenden Sie `az config param-persist`, um eine globale Variable festzulegen, die bei der Erstellung eines Azure-Speicherkontos verwendet wird.

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

Die CLI-Befehlsausgabe zeigt, dass ein neues Speicherkonto in der Ressourcengruppe unter der globalen Variablen „myGlobalVariableRG“ erstellt wurde.

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

Verwenden Sie `az config param-persist`, um permanente Parameter festzulegen, die bei der Erstellung eines Azure-Speicherkontos verwendet werden.  Wenn eine globale Variable für dasselbe Objekt festgelegt wird, wird die globale Variable durch den permanenten Parameter außer Kraft gesetzt.

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

Auch wenn eine globale Variable für die Ressourcengruppe mit dem Wert `myGlobalVariableRG` festgelegt ist und permanente Parameter aktiviert sind, wird das neue Speicherkonto mit `myParamPersistRG` erstellt.

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

## <a name="see-also"></a>Siehe auch

* [Tutorial: Verwenden von permanenten Parametern mit sequenziellen Azure CLI-Befehlen](param-persist-tutorial.md)
* [Azure CLI-Konfiguration mit „az configure“](azure-cli-configuration.md)

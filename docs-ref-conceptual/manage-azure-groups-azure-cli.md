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
# <a name="working-with-resource-groups-in-azure-cli"></a>Arbeiten mit Ressourcengruppen über die Azure CLI

Eine Azure-Ressourcengruppe ist ein Container, der verwandte Ressourcen für eine Azure-Lösung enthält. Eine Ressourcengruppe kann Speicher, virtuelle Computer, Apps, Dashboards, Dienste oder nahezu alle von Ihnen in Azure verwendeten Komponenten enthalten.

## <a name="create-a-resource-group"></a>Erstellen einer Ressourcengruppe

Verwenden Sie zum Erstellen einer Ressourcengruppe den Befehl [az group create](/cli/azure/group#az_group_create):

```azurecli
az group create --name MyResourceGroup --location eastus
```

Eine Ressourcengruppe gehört jeweils nur zu einem Standort. Führen Sie zum Anzeigen aller im aktuellen Abonnement unterstützten Standorte den Befehl [az account list-locations](/cli/azure/account#az_account_list_locations) aus:

```azurecli
az account list-locations
```

Verwenden Sie zum Anzeigen aller Ressourcengruppen für Ihr aktuelles Abonnement den Befehl [az group list](/cli/azure/group#az_group_list):

```azurecli
az group list --output table
```

> [!TIP]
> Der Parameter `--output` ist ein globaler Parameter und für alle Befehle verfügbar. Mit dem Wert **table** wird die Ausgabe in einem benutzerfreundlichen Format angezeigt. Weitere Informationen finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).

Wenn Sie eine Ressource erstellen, müssen Sie sie in einer Ressourcengruppe erstellen. Das folgende Beispiel zeigt ein mithilfe des Befehls [az storage account create](/cli/azure/storage/account#az_storage_account_create) erstelltes Speicherkonto:

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

Führen Sie zum Entfernen einer Ressourcengruppe den Befehl [az group delete](/cli/azure/group#az_group_delete) aus.

```azurecli
az group delete --name MyResourceGroup
```

Beim Entfernen einer Ressourcengruppe löschen Sie alle dazugehörigen Ressourcen. Es gibt keine Option, das Löschen von Ressourcen rückgängig zu machen. Wenn Sie einen der Befehle in diesem Artikel ausprobieren, wird beim Löschen der von Ihnen erstellten Ressourcengruppen Ihr Konto bereinigt.

## <a name="persist-a-resource-group"></a>Dauerhaftes Speichern einer Ressourcengruppe

Die Parameterpersistenz ermöglicht die Wiederverwendung von Werten für bestimmte Parameter, einschließlich Ressourcengruppen.

Aktivieren Sie zunächst das Persistenzfeature mithilfe des Befehls [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):

```azurecli
az config param-persist on
```

Erstellen Sie nach dem Aktivieren der Persistenz eine weitere Ressourcengruppe:

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

Solange Persistenz aktiviert ist, können Sie den Parameter `--resource-group` in künftigen Befehlen auslassen. Der folgende Befehl erstellt ein Speicherkonto in der Gruppe **OtherResourceGroup**.

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Wenn Sie eine Ressourcengruppe im Befehl angeben, hat dies Vorrang. Mit dem folgenden Befehl wird eine Speichergruppe in einer Ressourcengruppe namens **StorageGroups** erstellt:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

Wenn Sie jedoch eine andere Ressourcengruppe als Wert angeben, setzt die Azure CLI den dauerhaft gespeicherten Wert zurück. Neue Befehle verwenden **StorageGroups** als Ressourcengruppe. Die dauerhaft gespeicherten Werte können mit dem Befehl [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) angezeigt werden:

```azurecli
az config param-persist show
```

Mit diesem Befehl werden die aktuellen dauerhaft gespeicherten Werte angezeigt. Diese Werte werden in einer Datei namens *local_context_\<username>* in dem ausgeblendeten Verzeichnis *.azure* gespeichert. Die Azure CLI erstellt das Verzeichnis am aktuellen Standort, wenn Sie zum ersten Mal einen persistenten Wert erstellen.

Wenn Sie keine dauerhaft gespeicherten Parameter mehr verwenden möchten, führen Sie den Befehl [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) aus:

```azurecli
az config param-persist off
```

Von der Azure CLI werden die dauerhaft gespeicherten Werte gespeichert. Diese können in der lokalen Kontextdatei angezeigt werden. Wenn Sie die Parameterpersistenz erneut aktivieren, sind diese Werte bereits festgelegt.

Weitere Informationen zur Verwendung der Befehle vom Typ [az config param-persist](/cli/azure/config/param-persist) finden Sie unter [Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen](/cli/azure/param-persist-tutorial).

## <a name="set-a-default-resource-group"></a>Festlegen einer Standardressourcengruppe

Sie können eine Standardressourcengruppe für alle Befehle festlegen, die Sie über die lokale Azure CLI oder über Azure Cloud Shell ausführen. Die Azure CLI speichert diese Konfiguration lokal in einer Datei vom Typ *config*. Führen Sie zum Anzeigen der aktuellen Konfiguration den Befehl [az config get](/cli/azure/config#az_config_get) aus:

```azurecli
az config get
```

Im Ergebnis werden Standardressourcengruppen und andere Standardwerte angezeigt. Wenn Sie die Azure CLI zum ersten Mal verwenden, sind die Ergebnisse möglicherweise leer.

Führen Sie zum Festlegen einer Standardressourcengruppe für Ihre Azure CLI-Installation den Befehl [az config set](/cli/azure/config#az_config_set) aus:

```azurecli
az config set defaults.group=MyResourceGroup
```

Mit dem Befehl wird ein Wert für einen angegebenen Schlüssel festgelegt, in diesem Fall `defaults.group`. Informationen zu verfügbaren Konfigurationsoptionen finden Sie unter [Azure CLI-Konfiguration](/cli/azure/azure-cli-configuration).

> [!NOTE]
> Mit dem Befehl [az config set](/cli/azure/config#az_config_set) wird nicht überprüft, ob die von Ihnen eingegebene Ressourcengruppe vorhanden ist. Mit dem Befehl wird lediglich das Schlüssel-Wert-Paar gespeichert.

Nach dem Ausführen des Befehls erhalten Sie mit den folgenden beiden Befehlen dasselbe Ergebnis:

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

Eine Ressourcengruppe gehört zu einem Abonnement. Wenn Ihre Organisation über mehrere Abonnements verfügt, müssen Sie das entsprechende Abonnement festlegen, bevor Sie eine Ressourcengruppe im Abonnement verwenden. Gehört der Standardwert einer Ressourcengruppe nicht zu Ihrem aktuellen Abonnement, führt dies zu einem Fehler. Weitere Informationen zu mehreren Abonnements finden Sie unter [Verwenden mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md).

Sie müssen den Standardwert nicht zurücksetzen, um andere Ressourcengruppen zu verwenden. Geben Sie stattdessen die Ressourcengruppe an:

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

Der Standardwert gilt nur für Sie. Er wirkt sich nicht auf andere Benutzer oder auf Änderungen aus, die Sie über das Azure-Portal vornehmen.

Wenn Sie dauerhaft gespeicherte Parameterwerte wie in diesem Artikel beschrieben verwenden, haben diese Werte Vorrang vor den in der Datei *config* festgelegten Standardwerten.

## <a name="clean-up-resources"></a>Bereinigen von Ressourcen

Wenn Sie einen der Befehle in diesem Artikel ausprobiert haben, können Sie alle erstellten Ressourcen mithilfe des Befehls [az group delete](/cli/azure/group#az_group_delete) entfernen:

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

Mit diesem Befehl werden die Gruppe und gleichzeitig alle darin enthaltenen Ressourcen gelöscht.

Sie können die persistenten Parameter mithilfe des Befehls [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) entfernen:

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a>Siehe auch

[Azure CLI-Konfiguration](/cli/azure/azure-cli-configuration)

[Tutorial: Verwenden von permanenten Parametern zum Vereinfachen von sequenziellen Azure CLI-Befehlen](/cli/azure/param-persist-tutorial)

[Verwenden mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md)

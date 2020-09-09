---
title: Azure CLI-Referenzen für Azure IoT
description: Landing Page der Azure CLI-Referenzen für Azure IoT
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/05/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: paymaun.heidari
ms.custom: devx-track-azurecli
ms.openlocfilehash: 9190140c64f6a9863666329206839bb2553ffe79
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562786"
---
# <a name="azure-cli-for-azure-iot"></a>Azure CLI für Azure IoT

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](/cli/azure/what-is-azure-cli)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.  Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure IoT.  Es gibt mehr als 100 Referenzen für Azure IoT, die Sie bei der effektiven Verwendung von IoT-Diensten über eine Befehlszeile unterstützen.

## <a name="references-for-iot"></a>Referenzen für IoT

Die Azure IoT-CLI-Umgebung setzt sich aus zwei Teilen zusammen: aus der Azure CLI (in der Regel als CLI **Core** bezeichnet) und der Azure IoT-CLI-**Erweiterung**.

Bei den IoT-Funktionen in Azure CLI **Core** stehen Infrastrukturverwaltung und -konfiguration im Mittelpunkt. IoT Hub-CRUD-Vorgänge oder das Konfigurieren von IoT Hub-Nachrichtenrouten sind typische Anwendungsfälle für Core-Befehle.

Die IoT-**Erweiterung** bietet umfangreiche Features und Funktionen zum Verwalten und Bearbeiten von sowie zum Interagieren mit Daten, Entitäten und Objekten in der Infrastruktur selbst. Das Verwalten von Gerätebeständen, das Überwachen von Gerät-zu-Cloud-Ereignissen und das Aufrufen von Cloud-zu-Gerät-Methoden werden beispielsweise über die IoT-Erweiterung ermöglicht. Die Azure IoT-Erweiterung für die Azure CLI macht den Einsatz von experimentellen Technologien oder Vorabversionen möglich und trägt damit zu ihrer Vielseitigkeit in einer Vielzahl von Szenarien und Anwendungsfällen bei.

### <a name="core-reference-commands"></a>Core-Referenz – Befehle

| Verweis | Mit Erweiterung | BESCHREIBUNG
|-|-|-|
| [az iot](/cli/azure/iot) | ja  | Alle verfügbaren Azure CLI Core-Befehle für Azure IoT
| [az iot central](/cli/azure/iot/central) | ja | Verwalten von IoT Central-Objekten
| [az iot dps](/en-us/cli/azure/iot/dps) | ja | Verwalten von Device Provisioning Service in Azure IoT Hub
| [az iot hub](/cli/azure/iot/hub) | ja | Verwalten der Azure IoT Hub-Infrastruktur

### <a name="extension-reference-commands"></a>Erweiterungsreferenz – Befehle

| Verweis | Mit Core | BESCHREIBUNG
|-|-|-|
| [az iot](/cli/azure/ext/azure-iot/iot) | ja | Alle verfügbaren Azure CLI-Erweiterungsbefehle für Azure IoT
| [az iot central](/cli/azure/ext/azure-iot/iot/central) | ja | Verwalten von Azure Central-Lösungen und -Infrastrukturen (IoT Central)
| [az iot device](/cli/azure/ext/azure-iot/iot/device) | | Nutzen der Funktionen für Gerät-zu-Cloud- und Cloud-zu-Gerät-Messaging
| [az dt](/cli/azure/ext/azure-iot/dt) | | Verwalten von Azure Digital Twins-Lösungen und -Infrastrukturen
| [az iot dps](/cli/azure/ext/azure-iot/iot/dps) | ja | Verwalten von Entitäten in Device Provisioning Service in Azure IoT Hub
| [az iot edge](/cli/azure/ext/azure-iot/iot/edge) | | Verwalten von IoT-Lösungen am Edge
| [az iot hub](/cli/azure/ext/azure-iot/iot/hub) | ja | Verwalten von Entitäten in einer Azure IoT Hub-Instanz
| [az iot pnp](/cli/azure/ext/azure-iot/iot/pnp) | | Verwalten der Entitäten eines IoT Plug & Play-Modellrepositorys

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a>Weitere CLI-Befehle für von IoT verwendete Azure-Dienste

| Verweis | type | BESCHREIBUNG
|-|-|-|
| [az maps](/cli/azure/maps) | core | Verwalten von Azure Maps
| [az timeseriesinsights](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | Erweiterung | Verwalten von Azure Time Series Insights

### <a name="extension-reference-installation"></a>Erweiterungsreferenz – Installation

Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden.  Verwenden Sie den Befehl [az extension add](/cli/azure/azure-cli-extensions-overview), um eine Erweiterungsreferenz anhand des Namens zu installieren.  Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](/cli/azure/azure-cli-extensions-overview).

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a>Beliebte IoT-Artikel zur Azure CLI

- [Erstellen eines IoT Hubs mit der Azure-Befehlszeilenschnittstelle](/azure/iot-hub/iot-hub-create-using-cli)
- [Verwalten von IoT Central über Azure CLI](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [CLI-basierte Gerätetutorials mit Azure RTOS](/azure/rtos/getting-started?branch=master)
- [Verwenden der IoT-Erweiterung für Azure CLI für die Verwaltung von Azure IoT Hub-Geräten](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [Bedarfsgerechtes Bereitstellen und Überwachen von IoT Edge-Modulen mithilfe der Azure CLI](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [Schnellstart: Senden von Telemetriedaten von einem Gerät an einen IoT-Hub und Durchführen der Überwachung per Azure CLI](/azure/iot-hub/quickstart-send-telemetry-cli)
- [Tutorial: Konfigurieren des IoT Hub-Nachrichtenroutings mithilfe der Azure-Befehlszeilenschnittstelle](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [Installieren und Verwenden der Azure IoT-Erweiterung für die Azure CLI](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a>Azure CLI-Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.  Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure IoT benötigen Sie zunächst eine Ressourcengruppe.  Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Genauso einfach ist die Erstellung einer Azure IoT Hub-Instanz in der Region „westus“ im Tarif „Standard“.

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a>Weitere Informationen

- Unter [Erste Schritte mit der Azure CLI](/cli/azure/get-started-with-azure-cli) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [veröffentlichte Referenzen](/cli/azure/reference-index) und Referenzen zu [Erweiterungen](/cli/azure/azure-cli-extensions-list) in der Azure CLI-Dokumentation.

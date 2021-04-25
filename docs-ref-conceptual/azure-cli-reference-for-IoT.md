---
title: Azure CLI-Referenzen für Azure IoT
description: Landing Page der Azure CLI-Referenzen für Azure IoT
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 04/09/2021
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: paymaun.heidari
ms.custom: devx-track-azurecli
ms.openlocfilehash: cfa8569204409de81c27e8b9080ccd443a1f3224
ms.sourcegitcommit: f11f08a8b571d9909044693a8dc52c0cf2e9b2bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/19/2021
ms.locfileid: "107707698"
---
# <a name="azure-cli-for-azure-iot"></a>Azure CLI für Azure IoT

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen für zahlreiche Azure-Dienste zusammen. Für Azure IoT sind über 100 verschiedene Befehle verfügbar, mit denen Sie den Dienst effektiv über eine Befehlszeile verwenden können.

## <a name="references-for-iot"></a>Referenzen für IoT

Die [Azure IoT](/azure/iot-fundamentals/)-CLI-Umgebung setzt sich aus zwei Teilen zusammen: aus der Azure CLI (in der Regel als CLI-**Kern** bezeichnet) und der Azure IoT-CLI-**Erweiterung**.

Bei den IoT-Funktionen in Azure CLI **Core** stehen Infrastrukturverwaltung und -konfiguration im Mittelpunkt. IoT Hub-CRUD-Vorgänge oder das Konfigurieren von IoT Hub-Nachrichtenrouten sind typische Anwendungsfälle für Core-Befehle.

Die IoT-**Erweiterung** bietet umfangreiche Features und Funktionen zum Verwalten und Bearbeiten von sowie zum Interagieren mit Daten, Entitäten und Objekten in der Infrastruktur selbst. Das Verwalten von Gerätebeständen, das Überwachen von Gerät-zu-Cloud-Ereignissen und das Aufrufen von Cloud-zu-Gerät-Methoden werden beispielsweise über die IoT-Erweiterung ermöglicht. Die Azure IoT-Erweiterung für die Azure CLI macht den Einsatz von experimentellen Technologien oder Vorabversionen möglich und trägt damit zu ihrer Vielseitigkeit in einer Vielzahl von Szenarien und Anwendungsfällen bei. Die Erweiterung wird automatisch installiert, wenn Sie zum ersten Mal einen Erweiterungsverweis ausführen. Weitere Informationen zu Erweiterungsverweisen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

### <a name="reference-commands"></a>Verweisbefehle

> [!NOTE]
> Sie werden bei der ersten Verwendung aufgefordert, einen Erweiterungsverweis zu installieren. Alternativ können Sie den Befehl `az extension add` verwenden, um eine Erweiterung manuell zu installieren.

| Verweis | Kern oder Erweiterung | BESCHREIBUNG
|-|-|-|
| [az iot](/cli/azure/iot) | Beide  | Alle verfügbaren Azure CLI Core-Befehle für Azure IoT
| [az iot central](/cli/azure/iot/central) | Beide | Verwalten von IoT Central-Objekten
| [az iot device](/cli/azure/iot/device) | Erweiterung | Nutzen der Funktionen für Gerät-zu-Cloud- und Cloud-zu-Gerät-Messaging
| [az iot dps](/cli/azure/iot/dps) | Beide | Verwalten von Device Provisioning Service in Azure IoT Hub
| [az dt](/cli/azure/dt) | Erweiterung | Verwalten von Azure Digital Twins-Lösungen und -Infrastrukturen
| [az iot edge](/cli/azure/iot/edge) | Erweiterung | Verwalten von IoT-Lösungen am Edge
| [az iot hub](/cli/azure/iot/hub) | Beide | Verwalten der Azure IoT Hub-Infrastruktur
| [az iot product](/cli/azure/iot/product) | Erweiterung | Verwalten von Gerätetests für die Produktzertifizierung

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a>Weitere CLI-Befehle für von IoT verwendete Azure-Dienste

| Verweis | type | BESCHREIBUNG
|-|-|-|
| [az maps](/cli/azure/maps) | core | Verwalten von Azure Maps
| [az tsi](/cli/azure/tsi) | Erweiterung | Verwalten von Azure Time Series Insights

## <a name="popular-iot-articles-using-the-azure-cli"></a>Beliebte IoT-Artikel zur Azure CLI

- [Erstellen eines IoT Hubs mit der Azure-Befehlszeilenschnittstelle](/azure/iot-hub/iot-hub-create-using-cli)
- [Verwalten von IoT Central über Azure CLI](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [CLI-basierte Gerätetutorials mit Azure RTOS](/azure/rtos/getting-started?branch=master)
- [Verwenden der IoT-Erweiterung für Azure CLI für die Verwaltung von Azure IoT Hub-Geräten](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [Bedarfsgerechtes Bereitstellen und Überwachen von IoT Edge-Modulen mithilfe der Azure CLI](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [Senden von Telemetriedaten von einem Gerät an einen IoT-Hub und Durchführen der Überwachung per Azure CLI](/azure/iot-hub/quickstart-send-telemetry-cli)
- [Tutorial: Konfigurieren des IoT Hub-Nachrichtenroutings mithilfe der Azure-Befehlszeilenschnittstelle](/azure/iot-hub/tutorial-routing-config-message-routing-cli)

## <a name="azure-cli-reference-examples"></a>Azure CLI-Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, aber zur Verwendung der Azure CLI ist eine Befehlszeile erforderlich. Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure IoT benötigen Sie zunächst eine Ressourcengruppe. Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create --location westus --name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Die Erstellung einer Azure IoT Hub-Instanz ist ebenfalls ganz einfach.

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a>Weitere Informationen

- Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.

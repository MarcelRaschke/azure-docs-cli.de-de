---
title: Verfügbare Erweiterungen für die Azure CLI
description: Eine vollständige Liste mit den offiziell unterstützten Erweiterungen für die Azure CLI
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 09/24/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 97f682b95df3f080b5661ee361e75ef3e759d388
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177792"
---
# <a name="available-extensions-for-the-azure-cli"></a>Verfügbare Erweiterungen für die Azure CLI

Dieser Artikel enthält eine vollständige Liste mit den verfügbaren Erweiterungen für die Azure CLI, die von Microsoft angeboten und unterstützt werden.

Die Liste der Erweiterungen ist auch direkt über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli
az extension list-available --output table
```

| NAME | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Unterstützung für Befehlsaliase | JA |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.4.1 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.5.2 | Stellt die Befehlsebene der Datenebene für Azure IoT Hub, IoT Edge und den IoT Device Provisioning-Dienst bereit |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Fehlerbehebungen für Probleme im nativen botservice-CLI-Befehlsmodul. | JA |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. | JA |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.4.0 | Unterstützung für neue Database Migration Service-Szenarien. | JA |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Eine Azure CLI-Erweiterung für DNS-Zonen |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Unterstützung für Features von Azure EventGrid 2018-05-01-preview | JA |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Verwalten von benutzerdefinierten ExpressRoute-Verbindungen mithilfe einer ExpressRoute-Querverbindung |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.2.0 | Intelligentes Abfragen von CLI-Informationen | JA |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.8 | Unterstützung für das Kopieren verwalteter VM-Images zwischen Regionen |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | JA |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.2 | Unterstützung für Azure Log Analytics-Abfragefunktionen | JA |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Eine Azure CLI-Erweiterung für Verwaltungsgruppen |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.9.1 | Unterstützung für Microsoft Azure Service Fabric Mesh: Öffentliche Vorschau | JA |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Unterstützung für Virtual Network-Regeln in Azure MySQL- und Azure PostgreSQL-Ressourcen |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Unterstützung für das Abfragen von Azure-Ressourcen mit Resource Graph. | JA |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.1.6 | Zusätzliche Befehle für die Verwendung von SAP-HanaOnAzure-Instanzen. |  |
| [SignalR](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die SignalR-Verwaltung (Vorschauversion) | JA |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.4 | Bietet eine Vorschau für zukünftige Speicherfeatures. | JA |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Unterstützung für die Abonnementverwaltung (Vorschauversion) |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.8 | Eine Azure CLI-Erweiterung zum Verwalten von appservice-Ressourcen | JA |

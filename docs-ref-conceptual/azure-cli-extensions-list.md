---
title: Verfügbare Erweiterungen für die Azure CLI
description: Eine vollständige Liste mit den offiziell unterstützten Erweiterungen für die Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/27/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 2422d401d174ad779f8c9244dc2c966b5a9c53ef
ms.sourcegitcommit: d8e2fdc9b62d0a1d6b69b2483f68db31bd36e60f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "58524301"
---
# <a name="available-extensions-for-the-azure-cli"></a>Verfügbare Erweiterungen für die Azure CLI

Dieser Artikel enthält eine vollständige Liste mit den verfügbaren Erweiterungen für die Azure CLI, die von Microsoft unterstützt werden.

Die Liste der Erweiterungen ist auch über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli-interactive
az extension list-available --output table
```

| NAME | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.2.3 | Bietet eine Vorschau für zukünftige AKS-Features | Ja |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Unterstützung für Befehlsaliase | Ja |
| [anf-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/anf-preview) | 0.1.0 | Stellt eine Vorschau für neue Funktionen von Azure NetApp Files (ANF) bereit. | Ja |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Bietet eine Vorschau für zukünftige App-Konfigurationsfunktionen. | Ja |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.0 | Unterstützung für das Abfragen von Azure Application Insights-Metriken, -Ereignissen und -Protokollen | Ja |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 3.0.3 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.7.0 | Stellt die Befehlsebene der Datenebene für Azure IoT Hub, IoT Edge und den IoT Device Provisioning-Dienst bereit |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.4.0 | Tools zum Verwalten von Azure DevOps | Ja |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.1 | Verwalten von Azure Firewall-Ressourcen | Ja |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Fehlerbehebungen für Probleme im nativen botservice-CLI-Befehlsmodul. | Ja |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.10 | Zusätzliche Befehle zum Vereinfachen von Azure Database-Workflows. | Ja |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. | Ja |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.8.0 | Unterstützung für neue Database Migration Service-Szenarien. | Ja |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Eine Azure CLI-Erweiterung für DNS-Zonen |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Unterstützung für Features von Azure EventGrid 2018-09-15-preview | Ja |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Verwalten von Expressroute mit Previewfunktionen | Ja |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Verwalten von benutzerdefinierten ExpressRoute-Verbindungen mithilfe einer ExpressRoute-Querverbindung |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Intelligentes Abfragen von CLI-Informationen | Ja |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.3 | Verwalten von Front Door-Instanzen für Netzwerke | Ja |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.9 | Unterstützung für das Kopieren verwalteter VM-Images zwischen Regionen |  |
| [Interaktiv](https://github.com/Azure/azure-cli) | 0.4.1 | Interaktive Shell der Microsoft Azure-Befehlszeilenschnittstelle | Ja |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | Ja |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Unterstützung für Azure Log Analytics-Abfragefunktionen | Ja |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Eine Azure CLI-Erweiterung für Verwaltungsgruppen |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.4 | Unterstützung für Microsoft Azure Service Fabric Mesh: Öffentliche Vorschau | Ja |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Azure CLI-Erweiterung für Mixed Reality. |  |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Befehle zum Verwalten von privaten DNS-Zonen | Ja |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Unterstützung für Virtual Network-Regeln in Azure MySQL- und Azure PostgreSQL-Ressourcen |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Unterstützung für das Abfragen von Azure-Ressourcen mit Resource Graph. | Ja |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.3.4 | Zusätzliche Befehle für die Verwendung von SAP-HanaOnAzure-Instanzen. |  |
| [SignalR](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die SignalR-Verwaltung (Vorschauversion) | Ja |
| [sqlvm-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/sqlvm-preview) | 0.1.0 | Tools zum Verwalten von virtuellen SQL-Computern, Gruppen und Verfügbarkeitsgruppenlistenern | Ja |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.3 | Bietet eine Vorschau für zukünftige Speicherfeatures. | Ja |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Unterstützung für die Abonnementverwaltung (Vorschauversion) |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Verwalten von TAPs für virtuelle Netzwerke (VTAP) | Ja |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Verwalten von virtuellen WANs, Hubs, VPN-Gateways und VPN-Standorten | Ja |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.16 | Zusätzliche Befehle für Azure App Service | Ja |
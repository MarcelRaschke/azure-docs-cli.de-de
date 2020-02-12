---
title: Verfügbare Erweiterungen für die Azure CLI
description: Eine vollständige Liste mit den offiziell unterstützten Erweiterungen für die Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/05/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c11f43f2cabd0b7d2cef41cdecfead24791661e8
ms.sourcegitcommit: c332e9d6eeb4c0a8fbf587bd750002086f8ff0db
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/06/2020
ms.locfileid: "77038225"
---
# <a name="available-extensions-for-the-azure-cli"></a>Verfügbare Erweiterungen für die Azure CLI

Dieser Artikel enthält eine vollständige Liste mit den verfügbaren Erweiterungen für die Azure CLI, die von Microsoft unterstützt werden.

Die Liste der Erweiterungen ist auch über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli-interactive
az extension list-available --output table
```

| Name | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.27 | Bietet eine Vorschau für zukünftige AKS-Features | Ja |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Unterstützung für Befehlsaliase | Ja |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Bietet eine Vorschau für zukünftige App-Konfigurationsfunktionen. | Ja |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.3 | Unterstützung für die Verwaltung von Application Insights-Komponenten und die Abfrage von Metriken, Ereignissen und Protokollen von diesen Komponenten | Ja |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.9 | Die Azure IoT-Erweiterung für die Azure CLI |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.85 | AzureML-Befehlsmodul der Microsoft Azure-Befehlszeilentools |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.17.0 | Tools zum Verwalten von Azure DevOps |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.9 | Verwalten von Azure Firewall-Ressourcen | Ja |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Connectedmachine-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Erweiterung für Version 2 von Verbindungsmonitor der Microsoft Azure-Befehlszeile | Ja |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Zusätzliche Befehle zum Vereinfachen von Azure Database-Workflows. | Ja |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.4 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. | Ja |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Unterstützung für neue Database Migration Service-Szenarien. | Ja |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.4 | EventGrid-Befehlsmodul der Microsoft Azure-Befehlszeilentools | Ja |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Verwalten von Expressroute mit Previewfunktionen | Ja |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Verwalten von benutzerdefinierten ExpressRoute-Verbindungen mithilfe einer ExpressRoute-Querverbindung |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Intelligentes Abfragen von CLI-Informationen | Ja |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.2 | Verwalten von Front Door-Instanzen für Netzwerke |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.1 | Hack-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | HealthCareApis-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.3 | Unterstützung für das Kopieren verwalteter VM-Images zwischen Regionen |  |
| [Interaktiv](https://github.com/Azure/azure-cli) | 0.4.3 | Interaktive Shell der Microsoft Azure-Befehlszeilenschnittstelle | Ja |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc4 | Internet Analyzer-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | IpGroup-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | Ja |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Unterstützung für Azure Log Analytics-Abfragefunktionen | Ja |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Unterstützung für die Vorschauversion der Azure-Wartungsverwaltung | Ja |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Eine Azure CLI-Erweiterung für Verwaltungsgruppen |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Unterstützung für Microsoft Azure Service Fabric Mesh: Öffentliche Vorschau | Ja |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Azure CLI-Erweiterung für Mixed Reality. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Stellt eine Vorschau für neue Funktionen von Azure NetApp Files (ANF) bereit. | Ja |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Notification Hub-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc1 | Peering-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Befehle zum Verwalten von privaten DNS-Zonen | Ja |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Unterstützung für das Abfragen von Azure-Ressourcen mit Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Zusätzliche Befehle für die Verwendung von SAP-HanaOnAzure-Instanzen. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | spring-cloud-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Bietet eine Vorschau für zukünftige Speicherfeatures. | Ja |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Unterstützung für die Abonnementverwaltung (Vorschauversion) |  |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 0.1.0 | Support-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Verwalten von TAPs für virtuelle Netzwerke (VTAP) | Ja |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.2 | Verwalten von virtuellen WANs, Hubs, VPN-Gateways und VPN-Standorten | Ja |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.5 | Automatische Reparaturbefehle zur Problembehebung bei VMs |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.2.0 | Verwalten der Azure VMware-Lösung | Ja |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Zusätzliche Befehle für Azure App Service | Ja |
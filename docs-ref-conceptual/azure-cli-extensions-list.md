---
title: Verfügbare Erweiterungen für die Azure CLI
description: Eine vollständige Liste mit den offiziell unterstützten Erweiterungen für die Azure CLI
author: haroldrandom
ms.author: jianzen
manager: yonzhan,yungezz
ms.date: 08/28/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 117ffca4074f30b0ea7496f65f671446e0cfe6a9
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562820"
---
# <a name="available-extensions-for-the-azure-cli"></a>Verfügbare Erweiterungen für die Azure CLI

Dieser Artikel enthält eine vollständige Liste mit den verfügbaren Erweiterungen für die Azure CLI, die von Microsoft unterstützt werden.

Die Liste der Erweiterungen ist auch über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli-interactive
az extension list-available --output table
```

| Name | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [Konto](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | SubscriptionClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [ai-did-you-mean-this](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-did-you-mean-this) | 0.2.1 | Empfohlene Wiederherstellungsoptionen bei einem Fehler |  |
| [ai-examples](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-examples) | 0.2.3 | Hinzufügen von KI-gestützten Beispielen zum Hilfeinhalt. | Ja |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.61 | Bietet eine Vorschau für zukünftige AKS-Features | Ja |
| [alertsmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Warnungserweiterung der Microsoft Azure-Befehlszeilentools |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Unterstützung für Befehlsaliase | Ja |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.9 | Unterstützung für die Verwaltung von Application Insights-Komponenten und die Abfrage von Metriken, Ereignissen und Protokollen von diesen Komponenten | Ja |
| [attestation](https://github.com/Azure/azure-cli-extensions/tree/master/src/attestation) | 0.1.0 | AttestationManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 6.0.0 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.10 | Veraltet: Entfernen Sie „azure-cli-iot-ext“, und installieren Sie stattdessen die Erweiterung „azure-iot“. Die Legacyerweiterung „azure-cli-iot-ext“ wird am 15.09.2020 entfernt. |  |
| [azure-cli-ml](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py) | 1.12.0 | AzureML-Befehlsmodul der Microsoft Azure-Befehlszeilentools |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.18.0 | Tools zum Verwalten von Azure DevOps |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.5.1 | Verwalten von Azure Firewall-Ressourcen | Ja |
| [azure-iot](https://github.com/azure/azure-iot-cli-extension) | 0.9.8 | Die Azure IoT-Erweiterung für die Azure CLI |  |
| [blockchain](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | BlockchainManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [blueprint](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Blaupausenerweiterung der Microsoft Azure-Befehlszeilentools |  |
| [codespaces](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Die Codespaces-Erweiterung der Azure CLI | Ja |
| [connectedk8s](https://github.com/Azure/azure-cli-extensions) | 0.2.4 | Connectedk8s-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Connectedmachine-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Erweiterung für Version 2 von Verbindungsmonitor der Microsoft Azure-Befehlszeile | Ja |
| [costmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | CostManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [csvmware](https://github.com/Azure/az-vmware-cli) | 0.3.0 | Verwalten von Azure VMware Solution by CloudSimple | Ja |
| [custom-providers](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Erweiterung der Microsoft Azure-Befehlszeilentools für benutzerdefinierte Anbieter |  |
| [databox](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | DataBox-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [databricks](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | DatabricksClient-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [datafactory](https://github.com/Azure/azure-cli-extensions/tree/master/src/datafactory) | 0.1.0 | DataFactoryManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [datashare](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | DataShareManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.15 | Zusätzliche Befehle zum Vereinfachen von Azure Database-Workflows. | Ja |
| [deploy-to-azure](https://github.com/Azure/deploy-to-azure-cli-extension) | 0.2.0 | Bereitstellen in Azure mithilfe von GitHub-Aktionen | Ja |
| [desktopvirtualization](https://github.com/Azure/azure-cli-extensions/tree/master/src/desktopvirtualization) | 0.1.0 | DesktopVirtualizationAPIClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.5 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. | Ja |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.11.0 | Unterstützung für neue Database Migration Service-Szenarien. | Ja |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.9 | EventGrid-Befehlsmodul der Microsoft Azure-Befehlszeilentools | Ja |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Verwalten von Expressroute mit Previewfunktionen | Ja |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Verwalten von benutzerdefinierten ExpressRoute-Verbindungen mithilfe einer ExpressRoute-Querverbindung |  |
| [footprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/footprint) | 1.0.0 | FootprintMonitoringManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.9 | Verwalten von Front Door-Instanzen für Netzwerke |  |
| [guestconfig](https://github.com/Azure/azure-cli-extensions/tree/master/src/guestconfig) | 0.1.0 | GuestConfigurationClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.2 | Hack-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [hardware-security-modules](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | AzureDedicatedHSMResourceProvider-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | HealthcareApisManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [hpc-cache](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | StorageCache-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | Unterstützung für das Kopieren verwalteter VM-Images zwischen Regionen |  |
| [import-export](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | StorageImportExport-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [Interaktiv](https://github.com/Azure/azure-cli) | 0.4.4 | Interaktive Shell der Microsoft Azure-Befehlszeilenschnittstelle | Ja |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc5 | Internet Analyzer-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | IpGroup-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [k8sconfiguration](https://github.com/Azure/azure-cli-extensions) | 0.1.8 | K8sconfiguration-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | Ja |
| [kusto](https://github.com/Azure/azure-cli-extensions/tree/master/src/kusto) | 0.1.1 | KustoManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.2.1 | Unterstützung für Azure Log Analytics-Abfragefunktionen | Ja |
| [log-analytics-solution](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Unterstützung für die Azure Log Analytics-Lösung |  |
| [logic](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | LogicManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.1 | Unterstützung für die Azure-Wartungsverwaltung |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Unterstützung für Microsoft Azure Service Fabric Mesh: Öffentliche Vorschau | Ja |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Azure CLI-Erweiterung für Mixed Reality. | Ja |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Stellt eine Vorschau für neue Funktionen von Azure NetApp Files (ANF) bereit. | Ja |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Notification Hub-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | PeeringManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [portal](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Portal-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [powerbidedicated](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | PowerBIDedicated-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Befehle zum Verwalten von privaten DNS-Zonen | Ja |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.1.0 | Unterstützung für das Abfragen von Azure-Ressourcen mit Resource Graph. | Ja |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.6.4 | Zusätzliche Befehle für die Verwendung von SAP-HanaOnAzure-Instanzen. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | spring-cloud-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [storage-or-preview](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Erweiterung „Storage-ors-preview“ der Microsoft Azure-Befehlszeilentools | Ja |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.12 | Bietet eine Vorschau für zukünftige Speicherfeatures. | Ja |
| [storagesync](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | MicrosoftStorageSync-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [stream-analytics](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | stream-analytics-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.4 | Unterstützung für die Abonnementverwaltung (Vorschauversion) | Ja |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 1.0.2 | Support-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [synapse](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Synapse-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [timeseriesinsights](https://github.com/Azure/azure-cli-extensions/src/timeseriesinsights) | 0.1.2 | TimeSeriesInsightsClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Verwalten von TAPs für virtuelle Netzwerke (VTAP) | Ja |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.2.0 | Verwalten von virtuellen WANs, Hubs, VPN-Gateways und VPN-Standorten | Ja |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.3.2 | Automatische Reparaturbefehle zur Problembehebung bei VMs |  |
| [vmware](https://github.com/virtustream/azure-vmware-virtustream-cli-extension) | 0.6.0 | Vorschau der Befehle der Azure-VMware-Lösung | Ja |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Zusätzliche Befehle für Azure App Service | Ja |
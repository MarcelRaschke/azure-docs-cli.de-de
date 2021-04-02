---
title: Verfügbare Erweiterungen für die Azure CLI
description: Eine vollständige Liste mit den offiziell unterstützten Erweiterungen für die Azure CLI
author: haroldrandom
ms.author: jianzen
manager: yonzhan,yungezz
ms.date: 02/18/2021
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3e54f934770a71fff80ac063bdd41ccf74b3a673
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581341"
---
# <a name="available-extensions-for-the-azure-cli"></a>Verfügbare Erweiterungen für die Azure CLI

Dieser Artikel enthält eine vollständige Liste mit den verfügbaren Erweiterungen für die Azure CLI, die von Microsoft unterstützt werden.

Die Liste der Erweiterungen ist auch über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension#az_extension_list_available) aus:

```azurecli-interactive
az extension list-available --output table
```

| Name | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [Konto](https://github.com/Azure/azure-cli-extensions/tree/master/src/account) | 0.2.1 | SubscriptionClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [AD](https://github.com/Azure/azure-cli-extensions/tree/master/src/ad) | 0.1.0 | DomainServicesResourceProvider-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [ai-examples](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-examples) | 0.2.5 | Hinzufügen von KI-gestützten Beispielen zum Hilfeinhalt. | Ja |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.5.0 | Bietet eine Vorschau für zukünftige AKS-Features | Ja |
| [alertsmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Warnungserweiterung der Microsoft Azure-Befehlszeilentools |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Unterstützung für Befehlsaliase | Ja |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.13 | Unterstützung für die Verwaltung von Application Insights-Komponenten und die Abfrage von Metriken, Ereignissen und Protokollen von diesen Komponenten | Ja |
| [attestation](https://github.com/Azure/azure-cli-extensions/tree/master/src/attestation) | 0.2.0 | AttestationManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [automation](https://github.com/Azure/azure-cli-extensions/tree/master/src/automation) | 0.1.0 | AutomationClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 6.0.0 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-ml](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py) | 1.22.0.1 | AzureML-Befehlsmodul der Microsoft Azure-Befehlszeilentools |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.18.0 | Tools zum Verwalten von Azure DevOps |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.9.0 | Verwalten von Azure Firewall-Ressourcen | Ja |
| [azure-iot](https://github.com/azure/azure-iot-cli-extension) | 0.10.9 | Die Azure IoT-Erweiterung für die Azure CLI |  |
| [baremetal-infrastructure](https://github.com/Azure/azure-baremetalinfrastructure-cli-extension) | 0.0.2 | Zusätzliche Befehle für die Verwendung von BareMetal-Instanzen |  |
| [blockchain](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | BlockchainManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [blueprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/blueprint) | 0.2.1 | Blaupausenerweiterung der Microsoft Azure-Befehlszeilentools |  |
| [cli-translator](https://github.com/Azure/azure-cli-extensions/tree/master/src/cli-translator) | 0.3.0 | Übersetzen einer ARM-Vorlage in ausführbare Azure CLI-Skripts |  |
| [codespaces](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Die Codespaces-Erweiterung der Azure CLI | Ja |
| [communication](https://github.com/Azure/azure-cli-extensions/tree/master/src/communication) | 0.1.0 | CommunicationServiceManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [confluent](https://github.com/Azure/azure-cli-extensions/tree/master/src/confluent) | 0.1.0 | ConfluentManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [connectedk8s](https://github.com/Azure/azure-cli-extensions/tree/master/src/connectedk8s) | 0.2.9 | Connectedk8s-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions/tree/master/src/connectedmachine) | 0.3.0 | ConnectedMachine-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Erweiterung für Version 2 von Verbindungsmonitor der Microsoft Azure-Befehlszeile | Ja |
| [cosmosdb-preview](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Cosmosdb-preview-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [costmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | CostManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [csvmware](https://github.com/Azure/az-vmware-cli) | 0.3.0 | Verwalten von Azure VMware Solution by CloudSimple | Ja |
| [custom-providers](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Erweiterung der Microsoft Azure-Befehlszeilentools für benutzerdefinierte Anbieter |  |
| [databox](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | DataBox-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [databricks](https://github.com/Azure/azure-cli-extensions/tree/master/src/databricks) | 0.7.2 | DatabricksClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [datafactory](https://github.com/Azure/azure-cli-extensions/tree/master/src/datafactory) | 0.2.0 | DataFactoryManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [datashare](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | DataShareManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.2.1 | Zusätzliche Befehle zum Vereinfachen von Azure Database-Workflows. | Ja |
| [deploy-to-azure](https://github.com/Azure/deploy-to-azure-cli-extension) | 0.2.0 | Bereitstellen in Azure mithilfe von GitHub-Aktionen | Ja |
| [desktopvirtualization](https://github.com/Azure/azure-cli-extensions/tree/master/src/desktopvirtualization) | 0.1.0 | DesktopVirtualizationAPIClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions/tree/master/src/dev-spaces) | 1.0.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces ermöglicht eine schnelle, iterative Kubernetes-Bereitstellung für Teams. | Ja |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.12.0 | Unterstützung für neue Database Migration Service-Szenarien. | Ja |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.9 | EventGrid-Befehlsmodul der Microsoft Azure-Befehlszeilentools | Ja |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Verwalten von Expressroute mit Previewfunktionen | Ja |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Verwalten von benutzerdefinierten ExpressRoute-Verbindungen mithilfe einer ExpressRoute-Querverbindung |  |
| [footprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/footprint) | 1.0.0 | FootprintMonitoringManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.11 | Verwalten von Front Door-Instanzen für Netzwerke |  |
| [fzf](https://github.com/phealy/azure-cli-fzf) | 1.0.2 | fzf-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [guestconfig](https://github.com/Azure/azure-cli-extensions/tree/master/src/guestconfig) | 0.1.0 | GuestConfigurationClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [hack](https://github.com/Azure/azure-cli-extensions/tree/master/src/hack) | 0.4.3 | Hack-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [hardware-security-modules](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | AzureDedicatedHSMResourceProvider-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions/tree/master/src/healthcareapis) | 0.3.1 | HealthcareApisManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [hpc-cache](https://github.com/Azure/azure-cli-extensions/tree/master/src/hpc-cache) | 0.1.2 | StorageCache-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions/tree/master/src/image-copy) | 0.2.8 | Unterstützung für das Kopieren verwalteter VM-Images zwischen Regionen |  |
| [import-export](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | StorageImportExport-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [Interaktiv](https://github.com/Azure/azure-cli) | 0.4.4 | Interaktive Shell der Microsoft Azure-Befehlszeilenschnittstelle | Ja |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc5 | Internet Analyzer-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | IpGroup-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [k8sconfiguration](https://github.com/Azure/azure-cli-extensions/tree/master/src/k8sconfiguration) | 0.2.3 | K8sconfiguration-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | Ja |
| [kusto](https://github.com/Azure/azure-cli-extensions/tree/master/src/kusto) | 0.2.0 | KustoManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.2.2 | Unterstützung für Azure Log Analytics-Abfragefunktionen | Ja |
| [log-analytics-solution](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Unterstützung für die Azure Log Analytics-Lösung |  |
| [logic](https://github.com/Azure/azure-cli-extensions/tree/master/src/logic) | 0.1.2 | LogicManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [maintenance](https://github.com/Azure/azure-cli-extensions/tree/master/src/maintenance) | 1.1.0 | MaintenanceClient-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Unterstützung für Microsoft Azure Service Fabric Mesh: Öffentliche Vorschau | Ja |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Azure CLI-Erweiterung für Mixed Reality. | Ja |
| [monitor-control-service](https://github.com/Azure/azure-cli-extensions/tree/master/src/monitor-control-service) | 0.1.0 | MonitorClient-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Stellt eine Vorschau für neue Funktionen von Azure NetApp Files (ANF) bereit. | Ja |
| [Weiter](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Next-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Notification Hub-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [offazure](https://github.com/Azure/azure-cli-extensions/tree/master/src/offazure) | 0.1.0 | AzureMigrateV2-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | PeeringManagementClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [portal](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Portal-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [powerbidedicated](https://github.com/Azure/azure-cli-extensions/tree/master/src/powerbidedicated) | 0.2.0 | PowerBIDedicated-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Befehle zum Verwalten von privaten DNS-Zonen | Ja |
| [providerhub](https://github.com/Azure/azure-cli-extensions/tree/master/src/providerhub) | 0.1.0 | Providerhub-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [quantum](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Quantum-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.1.0 | Unterstützung für das Abfragen von Azure-Ressourcen mit Resource Graph. | Ja |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.6.4 | Zusätzliche Befehle für die Verwendung von SAP-HanaOnAzure-Instanzen. |  |
| [scheduled-query](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Scheduled_query-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [sentinel](https://github.com/Azure/azure-cli-extensions/tree/master/src/sentinel) | 0.1.0 | SecurityInsights-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions/tree/master/src/spring-cloud) | 2.1.1 | spring-cloud-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [ssh](https://github.com/Azure/azure-cli-extensions/tree/master/src/ssh) | 0.1.0 | SSH für VMs | Ja |
| [stack-hci](https://github.com/Azure/azure-cli-extensions/tree/master/src/stack-hci) | 0.1.2 | AzureStackHCIClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [storage-blob-preview](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Erweiterung „Storage-blob-preview“ der Microsoft Azure-Befehlszeilentools | Ja |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.7.0 | Bietet eine Vorschau für zukünftige Speicherfeatures. | Ja |
| [storagesync](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | MicrosoftStorageSync-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [stream-analytics](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | stream-analytics-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.4 | Unterstützung für die Abonnementverwaltung (Vorschauversion) | Ja |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 1.0.2 | Support-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [synapse](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Synapse-Erweiterung der Microsoft Azure-Befehlszeilentools | Ja |
| [timeseriesinsights](https://github.com/Azure/azure-cli-extensions/tree/master/src/timeseriesinsights) | 0.2.0 | TimeSeriesInsightsClient-Erweiterung der Microsoft Azure-Befehlszeilentools |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Verwalten von TAPs für virtuelle Netzwerke (VTAP) | Ja |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.2.4 | Verwalten von virtuellen WANs, Hubs, VPN-Gateways und VPN-Standorten | Ja |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.3.4 | Automatische Reparaturbefehle zur Problembehebung bei VMs |  |
| [vmware](https://github.com/Azure/az-vmware-cli) | 1.0.0 | Azure VMware Solution-Befehle |  |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.3.1 | Zusätzliche Befehle für Azure App Service | Ja |
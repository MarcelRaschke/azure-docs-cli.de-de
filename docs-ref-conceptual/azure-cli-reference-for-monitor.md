---
title: Azure CLI-Referenzen für Azure Monitor
description: Landing Page der Azure CLI-Referenzen für Azure Monitor
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: robb
ms.custom: devx-track-azurecli
ms.openlocfilehash: f2650a12fbcd976866e9b5d792db947baedb7fd5
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582106"
---
# <a name="azure-cli-for-azure-monitor"></a>Azure CLI für Azure Monitor

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.  Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure Monitor.  Es gibt mehr als 100 Referenzen für Azure Monitor, die Sie bei der effektiven Verwendung von Überwachungsdiensten über eine Befehlszeile unterstützen.

## <a name="references-for-azure-monitor"></a>Referenzen für Azure Monitor

Die [Azure Monitor](/azure/azure-monitor/)-CLI-Umgebung setzt sich aus zwei Teilen zusammen: aus der Azure CLI (in der Regel als CLI-**Core** bezeichnet) und der Azure Monitor-CLI-**Erweiterung**.  Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden. Mit dem Befehl [az extension add](/cli/azure/extension#az_extension_add) wird eine Erweiterungsreferenz anhand des Namens installiert.

> [!IMPORTANT]
>
> Azure Monitor enthält jetzt Application Insights und Log Analytics. Daher müssen Sie die Erweiterungen für jeden Unterbereich installieren, wenn Sie mit der Azure Monitor-CLI arbeiten.

### <a name="references"></a>References

| Verweis | Installieren der Erweiterung | BESCHREIBUNG | Weitere Informationen finden Sie unter
|-|-|-|-|
| [az monitor](/cli/azure/monitor) | | Die Befehlsgruppe der obersten Ebene für alle Azure CLI-Befehle für Azure Monitor. | [Azure Monitor – Übersicht](/azure/azure-monitor/overview)
| [az monitor action-group](/cli/azure/monitor/action-group) | | Verwalten von Aktionsgruppen, die sich auf Benachrichtigungen beziehen, sobald eine Warnung ausgelöst wurde. | [Azure Monitor-Warnungen](/azure/azure-monitor/platform/alerts-overview)
| [az monitor activity-log](/cli/azure/monitor/activity-log) | | Verwalten des Aktivitätsprotokolls einschließlich Aktivitätsprotokollwarnungen. | [Azure-Aktivitätsprotokolle](/azure/azure-monitor/platform/activity-log)
| [az monitor alert](/cli/azure/monitor/alert) | | NICHT für neue Entwicklungen verwenden.  Dieser Befehl verwaltet ältere klassische metrikbasierte Warnungsregeln, die mit Ausnahme weniger Fälle zu den neueren Metrikwarntypen migriert wurden. Verwenden Sie stattdessen [az monitor metrics alert](/cli/azure/monitor/metrics/alert). |
| [az monitor app-insights](/cli/azure/ext/application-insights/monitor/app-insights) | ja | Verwalten von Application Insights für die Anwendungsüberwachung. | [Application Insights-Übersicht](/azure/azure-monitor/app/app-insights-overview)
| [az monitor autoscale](/cli/azure/monitor/autoscale) | | Verwalten von Autoskalierungseinstellungen. | [Übersicht über Autoskalierung](/azure/azure-monitor/platform/autoscale-overview)
| [az monitor diagnostic-settings](/cli/azure/monitor/diagnostic-settings) | | Verwalten von Dienstdiagnoseeinstellungen, mit denen die Erfassung und das Routing zahlreicher Typen von Plattformmetriken und -protokollen eingerichtet werden. | [Erstellen von Diagnoseeinstellungen](/azure/azure-monitor/platform/diagnostic-settings)
| [az monitor log-analytics](/cli/azure/monitor/log-analytics) | | Verwalten von Protokollcluster und Arbeitsbereichen. | [Entwerfen Ihrer Azure Monitor-Protokollbereitstellung](/azure/azure-monitor/platform/design-logs-deployment)
| [az monitor log-analytics query](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | ja | Befehle zum Abfragen von Daten in Log Analytics-Arbeitsbereichen.  | [Erste Schritte mit Log Analytics-Abfragen](/azure/azure-monitor/log-query/get-started-portal)
| [az monitor log-profiles](/cli/azure/monitor/log-profiles) | | NICHT für neue Entwicklungen verwenden.  Dieser Befehl wurde bisher zum Weiterleiten von Aktivitätsprotokollen an Azure Monitor-Protokolle und Log Analytics verwendet.  Verwenden Sie stattdessen [Diagnoseeinstellungen](/azure/azure-monitor/platform/diagnostic-settings).  | [Senden eines Aktivitätsprotokolls an einen Log Analytics-Arbeitsbereich](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [az monitor metrics](/cli/azure/monitor/metrics) | | Verwalten von Plattformmetriken und Regeln für Metrikwarnungen nahezu in Echtzeit. | [Übersicht über Metriken in Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) und [Informationen zur Funktionsweise von Metrikwarnungen](/azure/azure-monitor/platform/alerts-metric-overview)
| [az monitor private-link-scope](/cli/azure/monitor/private-link-scope) | | Verwalten der Ressource des Azure Monitor-Private Link-Bereichs. | [Verwenden von Azure Private Link zum sicheren Verbinden von Netzwerken mit Azure Monitor](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a>Installieren von Erweiterungspaketen

Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden.  Mit dem Befehl [az extension add](./azure-cli-extensions-overview.md) wird eine Erweiterungsreferenz anhand des Namens installiert.

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a>Beliebte Monitor-Artikel zur Azure CLI

- [CLI-Beispiele für Azure Monitor](/azure/azure-monitor/samples/cli-samples)
- [Erstellen eines Log Analytics-Arbeitsbereichs mit der Azure CLI 2.0](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a>Azure CLI-Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.  Hier sehen Sie einige Codebeispiele, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure Monitor benötigen Sie zunächst eine Ressourcengruppe.  Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Das Erstellen einer Azure Monitor-Protokollwarnung ist ebenso unkompliziert.

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a>Weitere Informationen

- Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [veröffentlichte Referenzen](/cli/azure/reference-index) und Referenzen zu [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.

- Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

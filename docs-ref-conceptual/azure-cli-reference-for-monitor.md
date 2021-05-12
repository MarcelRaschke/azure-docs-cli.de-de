---
title: Azure CLI-Referenzen für Azure Monitor
description: Landing Page der Azure CLI-Referenzen für Azure Monitor
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 04/09/2021
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: robb
ms.custom: devx-track-azurecli
ms.openlocfilehash: 672834db4e49c5094a289ff1eb5d885b3c89ed70
ms.sourcegitcommit: f11f08a8b571d9909044693a8dc52c0cf2e9b2bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/19/2021
ms.locfileid: "107711064"
---
# <a name="azure-cli-for-azure-monitor"></a>Azure CLI für Azure Monitor

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen für zahlreiche Azure-Dienste zusammen. Für Azure Monitor sind über 100 verschiedene Befehle verfügbar, mit denen Sie den Dienst effektiv über eine Befehlszeile verwenden können.

## <a name="references-for-azure-monitor"></a>Referenzen für Azure Monitor

Die [Azure Monitor](/azure/azure-monitor/)-CLI-Umgebung setzt sich aus zwei Teilen zusammen: aus der Azure CLI (in der Regel als CLI-**Kern** bezeichnet) und der Azure Monitor-CLI-**Erweiterung** für den Speicherbedarf. Die Erweiterung wird automatisch installiert, wenn Sie zum ersten Mal einen Erweiterungsverweis ausführen. Weitere Informationen zu Erweiterungsverweisen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

> [!IMPORTANT]
>
> Azure Monitor enthält jetzt Application Insights und Log Analytics. Daher müssen Sie die Erweiterungen für jeden Unterbereich installieren, wenn Sie mit der Azure Monitor-CLI arbeiten.

### <a name="references"></a>References

> [!NOTE]
> Sie werden bei der ersten Verwendung aufgefordert, einen Erweiterungsverweis zu installieren. Alternativ können Sie den Befehl `az extension add` verwenden, um eine Erweiterung manuell zu installieren.

| Verweis | Installieren der Erweiterung | BESCHREIBUNG | Weitere Informationen finden Sie unter
|-|-|-|-|
| [az monitor](/cli/azure/monitor) | | Die Befehlsgruppe der obersten Ebene für alle Azure CLI-Befehle für Azure Monitor | [Azure Monitor – Übersicht](/azure/azure-monitor/overview)
| [az monitor action-group](/cli/azure/monitor/action-group) | | Verwalten von Aktionsgruppen, die sich auf Benachrichtigungen beziehen, sobald eine Warnung ausgelöst wurde. | [Azure Monitor-Warnungen](/azure/azure-monitor/platform/alerts-overview)
| [az monitor action-rule](/cli/azure/monitor/action-rule) | ja | Verwalten von Aktionsregeln, mit denen Sie die Aktionsgruppen für Ihre ausgelösten Warnungen hinzufügen oder unterdrücken können | [Azure Monitor-Warnungen](/azure/azure-monitor/alerts/alerts-action-rules)
| [az monitor activity-log](/cli/azure/monitor/activity-log) | | Verwalten von Aktivitätsprotokollen einschließlich Aktivitätsprotokollwarnungen | [Azure-Aktivitätsprotokolle](/azure/azure-monitor/platform/activity-log)
| [az monitor app-insights](/cli/azure/monitor/app-insights) | ja | Verwalten von Application Insights für die Anwendungsüberwachung. | [Application Insights-Übersicht](/azure/azure-monitor/app/app-insights-overview)
| [az monitor autoscale](/cli/azure/monitor/autoscale) | | Verwalten von Autoskalierungseinstellungen. | [Übersicht über Autoskalierung](/azure/azure-monitor/platform/autoscale-overview)
| [az monitor data-collection](/cli/azure/monitor/data-collection) | ja | Verwalten von Datensammlungsregeln | [Datensammlungsregeln in Azure Monitor (Vorschau)](/azure/azure-monitor/agents/data-collection-rule-overview)
| [az monitor diagnostic-settings](/cli/azure/monitor/diagnostic-settings) | | Verwalten von Dienstdiagnoseeinstellungen, mit denen die Erfassung und das Routing zahlreicher Typen von Plattformmetriken und -protokollen eingerichtet werden | [Erstellen von Diagnoseeinstellungen](/azure/azure-monitor/platform/diagnostic-settings)
| [az footprint](/cli/azure/footprint) | ja | Verwalten der Einstellungen für den Azure-Speicherbedarf |
| [az monitor log-analytics](/cli/azure/monitor/log-analytics) | | Verwalten von Protokollcluster und Arbeitsbereichen. | [Entwerfen Ihrer Azure Monitor-Protokollbereitstellung](/azure/azure-monitor/platform/design-logs-deployment)
| [az monitor log-analytics solution](/cli/azure/monitor/log-analytics/solution) | ja | Verwalten von Log Analytics-Lösungen |
| [az monitor log-profiles](/cli/azure/monitor/log-profiles) | | NICHT für neue Entwicklungen verwenden. Dieser Befehl wurde bisher zum Weiterleiten von Aktivitätsprotokollen an Azure Monitor-Protokolle und Log Analytics verwendet.  Verwenden Sie stattdessen [Diagnoseeinstellungen](/azure/azure-monitor/platform/diagnostic-settings).  | [Senden eines Aktivitätsprotokolls an einen Log Analytics-Arbeitsbereich](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [az monitor metrics](/cli/azure/monitor/metrics) | | Verwalten von Plattformmetriken und Regeln für Metrikwarnungen nahezu in Echtzeit. | [Übersicht über Metriken in Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) und [Informationen zur Funktionsweise von Metrikwarnungen](/azure/azure-monitor/platform/alerts-metric-overview)
| [az monitor private-link-scope](/cli/azure/monitor/private-link-scope) | | Verwalten der Ressourcen des Azure Monitor-Private Link-Bereichs | [Verwenden von Azure Private Link zum sicheren Verbinden von Netzwerken mit Azure Monitor](/azure/azure-monitor/platform/private-link-security)
| [az monitor scheduled-query](/cli/azure/monitor/scheduled-query) | ja | Verwalten geplanter Abfragen

## <a name="popular-monitor-articles-using-the-azure-cli"></a>Beliebte Monitor-Artikel zur Azure CLI

- [CLI-Beispiele für Azure Monitor](/azure/azure-monitor/samples/cli-samples)
- [Erstellen eines Log Analytics-Arbeitsbereichs mit Azure CLI 2.0](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a>Azure CLI-Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, aber zur Verwendung der Azure CLI ist eine Befehlszeile erforderlich. Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure Monitor benötigen Sie zunächst eine Ressourcengruppe.  Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create --location westus --name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Die Erstellung einer Azure Monitor-Protokollwarnung ist ebenfalls ganz einfach.

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a>Weitere Informationen

- Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.

- Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

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
ms.openlocfilehash: 064ba33fb9c10043d7b68e472a53332f44ac1283
ms.sourcegitcommit: 857d0f19fd87d37d134efdf0dda0e7003260938b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86308711"
---
# <a name="azure-cli-for-azure-monitor"></a><span data-ttu-id="23150-103">Azure CLI für Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="23150-103">Azure CLI for Azure Monitor</span></span>

<span data-ttu-id="23150-104">Die Azure-Befehlszeilenschnittstelle ([Azure CLI](/cli/azure/what-is-azure-cli)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.</span><span class="sxs-lookup"><span data-stu-id="23150-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="23150-105">Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="23150-105">It is available across many Azure services including Azure Monitor.</span></span>  <span data-ttu-id="23150-106">Es gibt mehr als 100 Referenzen für Azure Monitor, die Sie bei der effektiven Verwendung von Überwachungsdiensten über eine Befehlszeile unterstützen.</span><span class="sxs-lookup"><span data-stu-id="23150-106">There are over 100 references for Azure Monitor giving you the ability to work effectively with monitor services from a command line.</span></span>

## <a name="references-for-azure-monitor"></a><span data-ttu-id="23150-107">Referenzen für Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="23150-107">References for Azure Monitor</span></span>

<span data-ttu-id="23150-108">Die [Azure Monitor](/azure/azure-monitor/)-CLI-Umgebung setzt sich aus zwei Teilen zusammen: aus der Azure CLI (in der Regel als CLI-**Core** bezeichnet) und der Azure Monitor-CLI-**Erweiterung**.</span><span class="sxs-lookup"><span data-stu-id="23150-108">The [Azure Monitor](/azure/azure-monitor/) CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure Monitor CLI **extension**.</span></span>  <span data-ttu-id="23150-109">Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden.</span><span class="sxs-lookup"><span data-stu-id="23150-109">Azure CLI extension references must be installed prior to use.</span></span> <span data-ttu-id="23150-110">Mit dem Befehl [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) wird eine Erweiterungsreferenz anhand des Namens installiert.</span><span class="sxs-lookup"><span data-stu-id="23150-110">The [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) command installs an extension reference by name.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="23150-111">Azure Monitor enthält jetzt Application Insights und Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="23150-111">Azure Monitor now includes Application Insights and Log Analytics.</span></span> <span data-ttu-id="23150-112">Daher müssen Sie die Erweiterungen für jeden Unterbereich installieren, wenn Sie mit der Azure Monitor-CLI arbeiten.</span><span class="sxs-lookup"><span data-stu-id="23150-112">As such, you must install the extensions for each sub-area when working with Azure Monitor CLI.</span></span>

### <a name="references"></a><span data-ttu-id="23150-113">References</span><span class="sxs-lookup"><span data-stu-id="23150-113">References</span></span>

| <span data-ttu-id="23150-114">Verweis</span><span class="sxs-lookup"><span data-stu-id="23150-114">Reference</span></span> | <span data-ttu-id="23150-115">Installieren der Erweiterung</span><span class="sxs-lookup"><span data-stu-id="23150-115">Install extension</span></span> | <span data-ttu-id="23150-116">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="23150-116">Description</span></span> | <span data-ttu-id="23150-117">Weitere Informationen finden Sie unter</span><span class="sxs-lookup"><span data-stu-id="23150-117">For more information see</span></span>
|-|-|-|-|
| [<span data-ttu-id="23150-118">az monitor</span><span class="sxs-lookup"><span data-stu-id="23150-118">az monitor</span></span>](/cli/azure/monitor) | | <span data-ttu-id="23150-119">Die Befehlsgruppe der obersten Ebene für alle Azure CLI-Befehle für Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="23150-119">The top level command group for all Azure CLI commands for Azure Monitor.</span></span> | [<span data-ttu-id="23150-120">Azure Monitor – Übersicht</span><span class="sxs-lookup"><span data-stu-id="23150-120">Azure Monitor overview</span></span>](/azure/azure-monitor/overview)
| [<span data-ttu-id="23150-121">az monitor action-group</span><span class="sxs-lookup"><span data-stu-id="23150-121">az monitor action-group</span></span>](/cli/azure/monitor/action-group) | | <span data-ttu-id="23150-122">Verwalten von Aktionsgruppen, die sich auf Benachrichtigungen beziehen, sobald eine Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="23150-122">Manage action groups, which relate to notifications once an alert has fired.</span></span> | [<span data-ttu-id="23150-123">Azure Monitor-Warnungen</span><span class="sxs-lookup"><span data-stu-id="23150-123">Azure Monitor alerts</span></span>](/azure/azure-monitor/platform/alerts-overview)
| [<span data-ttu-id="23150-124">az monitor activity-log</span><span class="sxs-lookup"><span data-stu-id="23150-124">az monitor activity-log</span></span>](/cli/azure/monitor/activity-log) | | <span data-ttu-id="23150-125">Verwalten des Aktivitätsprotokolls einschließlich Aktivitätsprotokollwarnungen.</span><span class="sxs-lookup"><span data-stu-id="23150-125">Manage activity log including activity log alerts.</span></span> | [<span data-ttu-id="23150-126">Azure-Aktivitätsprotokolle</span><span class="sxs-lookup"><span data-stu-id="23150-126">Azure activity logs</span></span>](/azure/azure-monitor/platform/activity-log)
| [<span data-ttu-id="23150-127">az monitor alert</span><span class="sxs-lookup"><span data-stu-id="23150-127">az monitor alert</span></span>](/cli/azure/monitor/alert) | | <span data-ttu-id="23150-128">NICHT für neue Entwicklungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="23150-128">DO NOT USE for new development.</span></span>  <span data-ttu-id="23150-129">Dieser Befehl verwaltet ältere klassische metrikbasierte Warnungsregeln, die mit Ausnahme weniger Fälle zu den neueren Metrikwarntypen migriert wurden.</span><span class="sxs-lookup"><span data-stu-id="23150-129">This command manages older classic metric-based alert rules, which in all but a few cases have been migrated to the newer metric alert types.</span></span> <span data-ttu-id="23150-130">Verwenden Sie stattdessen [az monitor metrics alert](/cli/azure/monitor/metrics/alert).</span><span class="sxs-lookup"><span data-stu-id="23150-130">Use [az monitor metrics alert](/cli/azure/monitor/metrics/alert) instead.</span></span> |
| [<span data-ttu-id="23150-131">az monitor app-insights</span><span class="sxs-lookup"><span data-stu-id="23150-131">az monitor app-insights</span></span>](/cli/azure/ext/application-insights/monitor/app-insights) | <span data-ttu-id="23150-132">ja</span><span class="sxs-lookup"><span data-stu-id="23150-132">yes</span></span> | <span data-ttu-id="23150-133">Verwalten von Application Insights für die Anwendungsüberwachung.</span><span class="sxs-lookup"><span data-stu-id="23150-133">Manage Application Insights for application monitoring.</span></span> | [<span data-ttu-id="23150-134">Application Insights-Übersicht</span><span class="sxs-lookup"><span data-stu-id="23150-134">Application insights overview</span></span>](/azure/azure-monitor/app/app-insights-overview)
| [<span data-ttu-id="23150-135">az monitor autoscale</span><span class="sxs-lookup"><span data-stu-id="23150-135">az monitor autoscale</span></span>](/cli/azure/monitor/autoscale) | | <span data-ttu-id="23150-136">Verwalten von Autoskalierungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="23150-136">Manage autoscale settings.</span></span> | [<span data-ttu-id="23150-137">Übersicht über Autoskalierung</span><span class="sxs-lookup"><span data-stu-id="23150-137">Autoscale overview</span></span>](/azure/azure-monitor/platform/autoscale-overview)
| [<span data-ttu-id="23150-138">az monitor diagnostic-settings</span><span class="sxs-lookup"><span data-stu-id="23150-138">az monitor diagnostic-settings</span></span>](/cli/azure/monitor/diagnostic-settings) | | <span data-ttu-id="23150-139">Verwalten von Dienstdiagnoseeinstellungen, mit denen die Erfassung und das Routing zahlreicher Typen von Plattformmetriken und -protokollen eingerichtet werden.</span><span class="sxs-lookup"><span data-stu-id="23150-139">Manage service diagnostic settings, which sets up collection and routing of many types of platform metrics and logs.</span></span> | [<span data-ttu-id="23150-140">Erstellen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="23150-140">Create diagnostic settings</span></span>](/azure/azure-monitor/platform/diagnostic-settings)
| [<span data-ttu-id="23150-141">az monitor log-analytics</span><span class="sxs-lookup"><span data-stu-id="23150-141">az monitor log-analytics</span></span>](/cli/azure/monitor/log-analytics) | | <span data-ttu-id="23150-142">Verwalten von Protokollcluster und Arbeitsbereichen.</span><span class="sxs-lookup"><span data-stu-id="23150-142">Manage log clusters and work spaces.</span></span> | [<span data-ttu-id="23150-143">Entwerfen Ihrer Azure Monitor-Protokollbereitstellung</span><span class="sxs-lookup"><span data-stu-id="23150-143">Designing your Azure Monitor Logs deployment</span></span>](/azure/azure-monitor/platform/design-logs-deployment)
| [<span data-ttu-id="23150-144">az monitor log-analytics query</span><span class="sxs-lookup"><span data-stu-id="23150-144">az monitor log-analytics query</span></span>](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | <span data-ttu-id="23150-145">ja</span><span class="sxs-lookup"><span data-stu-id="23150-145">yes</span></span> | <span data-ttu-id="23150-146">Befehle zum Abfragen von Daten in Log Analytics-Arbeitsbereichen.</span><span class="sxs-lookup"><span data-stu-id="23150-146">Commands for querying data in Log Analytics workspaces.</span></span>  | [<span data-ttu-id="23150-147">Erste Schritte mit Log Analytics-Abfragen</span><span class="sxs-lookup"><span data-stu-id="23150-147">Get started with Log Analytics queries</span></span>](/azure/azure-monitor/log-query/get-started-portal)
| [<span data-ttu-id="23150-148">az monitor log-profiles</span><span class="sxs-lookup"><span data-stu-id="23150-148">az monitor log-profiles</span></span>](/cli/azure/monitor/log-profiles) | | <span data-ttu-id="23150-149">NICHT für neue Entwicklungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="23150-149">DO NOT USE for new development.</span></span>  <span data-ttu-id="23150-150">Dieser Befehl wurde bisher zum Weiterleiten von Aktivitätsprotokollen an Azure Monitor-Protokolle und Log Analytics verwendet.</span><span class="sxs-lookup"><span data-stu-id="23150-150">This command was previously used to route activity logs to Azure Monitor Logs and Log Analytics.</span></span>  <span data-ttu-id="23150-151">Verwenden Sie stattdessen [Diagnoseeinstellungen](/azure/azure-monitor/platform/diagnostic-settings).</span><span class="sxs-lookup"><span data-stu-id="23150-151">Use [diagnostic settings](/azure/azure-monitor/platform/diagnostic-settings) instead.</span></span>  | [<span data-ttu-id="23150-152">Senden eines Aktivitätsprotokolls an einen Log Analytics-Arbeitsbereich</span><span class="sxs-lookup"><span data-stu-id="23150-152">Send the Activity log to a Log Analytics workspace</span></span>](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [<span data-ttu-id="23150-153">az monitor metrics</span><span class="sxs-lookup"><span data-stu-id="23150-153">az monitor metrics</span></span>](/cli/azure/monitor/metrics) | | <span data-ttu-id="23150-154">Verwalten von Plattformmetriken und Regeln für Metrikwarnungen nahezu in Echtzeit.</span><span class="sxs-lookup"><span data-stu-id="23150-154">Manage platform metrics and near-realtime metric alert rules.</span></span> | <span data-ttu-id="23150-155">[Übersicht über Metriken in Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) und [Informationen zur Funktionsweise von Metrikwarnungen](/azure/azure-monitor/platform/alerts-metric-overview)</span><span class="sxs-lookup"><span data-stu-id="23150-155">[Overview of metrics in Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) and [Understand how metric alerts work](/azure/azure-monitor/platform/alerts-metric-overview)</span></span>
| [<span data-ttu-id="23150-156">az monitor private-link-scope</span><span class="sxs-lookup"><span data-stu-id="23150-156">az monitor private-link-scope</span></span>](/cli/azure/monitor/private-link-scope) | | <span data-ttu-id="23150-157">Verwalten der Ressource des Azure Monitor-Private Link-Bereichs.</span><span class="sxs-lookup"><span data-stu-id="23150-157">Manage monitor private link scope resource.</span></span> | [<span data-ttu-id="23150-158">Verwenden von Azure Private Link zum sicheren Verbinden von Netzwerken mit Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="23150-158">Use Azure Private Link to securely connect networks to Azure Monitor</span></span>](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a><span data-ttu-id="23150-159">Installieren von Erweiterungspaketen</span><span class="sxs-lookup"><span data-stu-id="23150-159">Installing extension references</span></span>

<span data-ttu-id="23150-160">Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden.</span><span class="sxs-lookup"><span data-stu-id="23150-160">Azure CLI extension references must be installed prior to use.</span></span>  <span data-ttu-id="23150-161">Mit dem Befehl [az extension add](/cli/azure/azure-cli-extensions-overview) wird eine Erweiterungsreferenz anhand des Namens installiert.</span><span class="sxs-lookup"><span data-stu-id="23150-161">The [az extension add](/cli/azure/azure-cli-extensions-overview) command installs an extension reference by name.</span></span>

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a><span data-ttu-id="23150-162">Beliebte Monitor-Artikel zur Azure CLI</span><span class="sxs-lookup"><span data-stu-id="23150-162">Popular Monitor articles using the Azure CLI</span></span>

- [<span data-ttu-id="23150-163">CLI-Beispiele für Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="23150-163">Azure Monitor CLI samples</span></span>](/azure/azure-monitor/samples/cli-samples)
- [<span data-ttu-id="23150-164">Erstellen eines Log Analytics-Arbeitsbereichs mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="23150-164">Create a Log Analytics workspace with Azure CLI 2.0</span></span>](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="23150-165">Azure CLI-Referenzbeispiele</span><span class="sxs-lookup"><span data-stu-id="23150-165">Azure CLI reference examples</span></span>

<span data-ttu-id="23150-166">Es stehen Beispiele für jede Azure CLI-Referenz bereit.</span><span class="sxs-lookup"><span data-stu-id="23150-166">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="23150-167">Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23150-167">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="23150-168">Hier sehen Sie einige Codebeispiele, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.</span><span class="sxs-lookup"><span data-stu-id="23150-168">Here are a few code samples to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="23150-169">Zum Arbeiten mit Azure Monitor benötigen Sie zunächst eine Ressourcengruppe.</span><span class="sxs-lookup"><span data-stu-id="23150-169">To work with Azure Monitor, you'll first need a resource group.</span></span>  <span data-ttu-id="23150-170">Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="23150-170">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="23150-171">Das Erstellen einer Azure Monitor-Protokollwarnung ist ebenso unkompliziert.</span><span class="sxs-lookup"><span data-stu-id="23150-171">Creating an Azure Monitor log alert is just as straightforward.</span></span>

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="23150-172">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="23150-172">See also</span></span>

- <span data-ttu-id="23150-173">Unter [Erste Schritte mit der Azure CLI](/cli/azure/get-started-with-azure-cli) erhalten Sie Informationen zur Installation und Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="23150-173">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="23150-174">Entdecken Sie weitere [veröffentlichte Referenzen](/cli/azure/reference-index) und Referenzen zu [Erweiterungen](/cli/azure/azure-cli-extensions-list) in der Azure CLI-Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="23150-174">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>

- <span data-ttu-id="23150-175">Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="23150-175">Learn more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>
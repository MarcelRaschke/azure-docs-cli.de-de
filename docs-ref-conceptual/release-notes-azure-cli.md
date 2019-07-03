---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/18/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8431946b169b550bfd3f5120cf26e2feeb5c9f2c
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194861"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f138f-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f138f-103">Azure CLI release notes</span></span>

## <a name="june-18-2019"></a><span data-ttu-id="f138f-104">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-104">June 18, 2019</span></span>

<span data-ttu-id="f138f-105">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="f138f-105">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="f138f-106">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-106">Core</span></span>

<span data-ttu-id="f138f-107">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="f138f-107">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="f138f-108">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-108">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="f138f-109">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="f138f-109">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="f138f-110">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="f138f-110">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="f138f-111">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="f138f-111">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="f138f-112">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="f138f-112">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="f138f-113">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="f138f-113">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-114">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-114">ACR</span></span>
* <span data-ttu-id="f138f-115">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-115">Added 'acr check-health' command</span></span>
* <span data-ttu-id="f138f-116">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="f138f-116">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-117">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-117">ACS</span></span>
* <span data-ttu-id="f138f-118">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="f138f-118">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-119">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-119">AMS</span></span>
* <span data-ttu-id="f138f-120">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="f138f-120">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-121">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-121">AppService</span></span>
* <span data-ttu-id="f138f-122">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-122">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="f138f-123">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-123">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="f138f-124">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-124">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="f138f-125">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-125">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="f138f-126">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-126">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="f138f-127">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-127">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-128">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-128">Batch</span></span>
* <span data-ttu-id="f138f-129">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-129">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-130">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f138f-130">BatchAI</span></span>
* <span data-ttu-id="f138f-131">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="f138f-131">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-132">BotService</span><span class="sxs-lookup"><span data-stu-id="f138f-132">BotService</span></span>
* <span data-ttu-id="f138f-133">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-133">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-134">CosmosDB</span></span>
* <span data-ttu-id="f138f-135">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="f138f-135">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="f138f-136">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="f138f-136">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="f138f-137">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-137">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="f138f-138">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="f138f-138">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f138f-139">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f138f-139">EventGrid</span></span>
* <span data-ttu-id="f138f-140">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-140">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="f138f-141">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-141">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="f138f-142">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-142">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="f138f-143">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-143">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="f138f-144">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-144">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f138f-145">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f138f-145">HDInsight</span></span>
* <span data-ttu-id="f138f-146">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-146">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-147">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-147">IoT</span></span>
* <span data-ttu-id="f138f-148">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-148">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="f138f-149">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-149">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="f138f-150">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-150">Network</span></span>
* <span data-ttu-id="f138f-151">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-151">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="f138f-152">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-152">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="f138f-153">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-153">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="f138f-154">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-154">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-155">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-155">Resource</span></span>
* <span data-ttu-id="f138f-156">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-156">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="f138f-157">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-157">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="f138f-158">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f138f-158">ServiceBus</span></span>
* <span data-ttu-id="f138f-159">Problem mit `servicebus topic create --max-size` behoben [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="f138f-159">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-160">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-160">SQL</span></span>
* <span data-ttu-id="f138f-161">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="f138f-161">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="f138f-162">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-162">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="f138f-163">SQLVm</span><span class="sxs-lookup"><span data-stu-id="f138f-163">SQLVm</span></span>
* <span data-ttu-id="f138f-164">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="f138f-164">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="f138f-165">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-165">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-166">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-166">Storage</span></span>
* <span data-ttu-id="f138f-167">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-167">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="f138f-168">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-168">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-169">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-169">VM</span></span>
* <span data-ttu-id="f138f-170">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-170">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="f138f-171">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-171">June 4, 2019</span></span>

<span data-ttu-id="f138f-172">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="f138f-172">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="f138f-173">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-173">Core</span></span>
* <span data-ttu-id="f138f-174">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-174">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-175">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-175">ACR</span></span>
* <span data-ttu-id="f138f-176">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-176">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-177">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-177">ACS</span></span>
* <span data-ttu-id="f138f-178">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="f138f-178">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="f138f-179">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="f138f-179">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-180">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-180">Batch</span></span>
* <span data-ttu-id="f138f-181">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="f138f-181">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-182">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-182">IoT</span></span>
* <span data-ttu-id="f138f-183">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-183">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="f138f-184">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-184">Network</span></span>
* <span data-ttu-id="f138f-185">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-185">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="f138f-186">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-186">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="f138f-187">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-187">Resource</span></span>
* <span data-ttu-id="f138f-188">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f138f-188">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="f138f-189">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-189">Role</span></span>
* <span data-ttu-id="f138f-190">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-190">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="f138f-191">Compute</span><span class="sxs-lookup"><span data-stu-id="f138f-191">Compute</span></span>
* <span data-ttu-id="f138f-192">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="f138f-192">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="f138f-193">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-193">May 21, 2019</span></span>

<span data-ttu-id="f138f-194">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="f138f-194">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="f138f-195">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-195">Core</span></span>
* <span data-ttu-id="f138f-196">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-196">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="f138f-197">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="f138f-197">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="f138f-198">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="f138f-198">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-199">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-199">ACR</span></span>
* <span data-ttu-id="f138f-200">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-200">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-201">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-201">ACS</span></span>
* <span data-ttu-id="f138f-202">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-202">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-203">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-203">AppService</span></span>
* <span data-ttu-id="f138f-204">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-204">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="f138f-205">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="f138f-205">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="f138f-206">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="f138f-206">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="f138f-207">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-207">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="f138f-208">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f138f-208">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="f138f-209">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="f138f-209">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="f138f-210">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="f138f-210">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-211">BotService</span><span class="sxs-lookup"><span data-stu-id="f138f-211">BotService</span></span>
* <span data-ttu-id="f138f-212">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f138f-212">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="f138f-213">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-213">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-214">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-214">Consumption</span></span>
* <span data-ttu-id="f138f-215">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-215">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-216">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-216">IoT</span></span>
* <span data-ttu-id="f138f-217">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-217">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="f138f-218">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-218">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="f138f-220">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-220">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="f138f-221">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="f138f-221">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-222">RDBMS</span></span>
* <span data-ttu-id="f138f-223">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-223">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="f138f-224">RBAC</span><span class="sxs-lookup"><span data-stu-id="f138f-224">RBAC</span></span>
* <span data-ttu-id="f138f-225">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-225">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-226">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-226">Storage</span></span>
* <span data-ttu-id="f138f-227">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-227">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="f138f-228">Compute</span><span class="sxs-lookup"><span data-stu-id="f138f-228">Compute</span></span>
* <span data-ttu-id="f138f-229">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-229">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="f138f-230">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-230">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="f138f-231">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="f138f-231">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="f138f-232">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-232">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="f138f-233">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-233">May 6, 2019</span></span>

<span data-ttu-id="f138f-234">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="f138f-234">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-235">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-235">ACS</span></span>
* <span data-ttu-id="f138f-236">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-236">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="f138f-237">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-237">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="f138f-238">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-238">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="f138f-239">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-239">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-240">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-240">Appservice</span></span>
* <span data-ttu-id="f138f-241">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f138f-241">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="f138f-242">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="f138f-242">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="f138f-243">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="f138f-243">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="f138f-244">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-244">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="f138f-245">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-245">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="f138f-246">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-246">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="f138f-247">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-247">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="f138f-248">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="f138f-248">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="f138f-249">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-249">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="f138f-250">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-250">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-251">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-251">Batch</span></span>
* <span data-ttu-id="f138f-252">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-252">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-253">Botservice</span><span class="sxs-lookup"><span data-stu-id="f138f-253">Botservice</span></span>
* <span data-ttu-id="f138f-254">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="f138f-254">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="f138f-255">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-255">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="f138f-256">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-256">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="f138f-257">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="f138f-257">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="f138f-258">[BREAKING CHANGE] `--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-258">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="f138f-259">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="f138f-259">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="f138f-260">[BREAKING CHANGE] `--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-260">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="f138f-261">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-261">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="f138f-262">[BREAKING CHANGE] `bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-262">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="f138f-263">[BREAKING CHANGE] `bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f138f-263">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="f138f-264">[BREAKING CHANGE] `bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="f138f-264">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="f138f-265">[BREAKING CHANGE] `--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="f138f-265">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="f138f-266">[BREAKING CHANGE] `Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-266">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="f138f-267">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-267">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="f138f-268">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="f138f-268">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="f138f-269">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-269">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="f138f-270">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-270">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f138f-271">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="f138f-271">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="f138f-272">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="f138f-272">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="f138f-273">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-273">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f138f-274">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-274">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="f138f-275">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f138f-275">Configure</span></span>
* <span data-ttu-id="f138f-276">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-276">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f138f-277">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f138f-277">Eventhubs</span></span>
* <span data-ttu-id="f138f-278">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-278">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f138f-279">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-279">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-280">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-280">Network</span></span>
* <span data-ttu-id="f138f-281">[BREAKING CHANGE] `--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f138f-281">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="f138f-282">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f138f-282">Policy Insights</span></span>
* <span data-ttu-id="f138f-283">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-283">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="f138f-284">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-284">Role</span></span>
* <span data-ttu-id="f138f-285">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-285">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="f138f-286">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f138f-286">Service Bus</span></span>
* <span data-ttu-id="f138f-287">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-287">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f138f-288">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-288">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="f138f-289">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f138f-289">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-290">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-290">SQL</span></span>
* <span data-ttu-id="f138f-291">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-291">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-292">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-292">VM</span></span>
* <span data-ttu-id="f138f-293">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="f138f-293">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="f138f-294">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="f138f-294">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="f138f-295">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-295">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="f138f-296">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-296">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="f138f-297">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-297">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="f138f-298">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-298">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="f138f-299">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-299">April 23, 2019</span></span>

<span data-ttu-id="f138f-300">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="f138f-300">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-301">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-301">ACS</span></span>
* <span data-ttu-id="f138f-302">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-302">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="f138f-303">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-303">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-304">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-304">AMS</span></span>
* <span data-ttu-id="f138f-305">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-305">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-306">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-306">AppService</span></span>
* <span data-ttu-id="f138f-307">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-307">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="f138f-308">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-308">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="f138f-309">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f138f-309">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="f138f-310">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f138f-310">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="f138f-311">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-311">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="f138f-312">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-312">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="f138f-313">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f138f-313">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="f138f-314">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="f138f-314">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="f138f-315">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f138f-315">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="f138f-316">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="f138f-316">Deployment Manager</span></span>
* <span data-ttu-id="f138f-317">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-317">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="f138f-318">Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-318">Lab</span></span>
* <span data-ttu-id="f138f-319">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="f138f-319">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="f138f-320">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-320">Network</span></span>
* <span data-ttu-id="f138f-321">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-321">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-322">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-322">Resource</span></span>
* <span data-ttu-id="f138f-323">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-323">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="f138f-324">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="f138f-324">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="f138f-325">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-325">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="f138f-326">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-326">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-327">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-327">SQL</span></span>
* <span data-ttu-id="f138f-328">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-328">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="f138f-329">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f138f-329">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="f138f-330">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-330">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="f138f-331">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-331">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-332">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-332">Storage</span></span>
* <span data-ttu-id="f138f-333">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-333">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-334">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-334">VM</span></span>
* <span data-ttu-id="f138f-335">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-335">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="f138f-336">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-336">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="f138f-337">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f138f-337">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="f138f-338">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-338">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="f138f-339">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-339">Core</span></span>
* <span data-ttu-id="f138f-340">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-340">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-341">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-341">ACR</span></span>
* <span data-ttu-id="f138f-342">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-342">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-343">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-343">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="f138f-346">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-346">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="f138f-347">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-347">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-348">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-348">AppService</span></span>
* <span data-ttu-id="f138f-349">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-349">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="f138f-350">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-350">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="f138f-351">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-351">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="f138f-352">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="f138f-352">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="f138f-353">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-353">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="f138f-354">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-354">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="f138f-355">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-355">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-356">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-356">CDN</span></span>
* <span data-ttu-id="f138f-357">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="f138f-357">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="f138f-358">Feedback</span><span class="sxs-lookup"><span data-stu-id="f138f-358">Feedback</span></span>
* <span data-ttu-id="f138f-359">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-359">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="f138f-360">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="f138f-360">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="f138f-361">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="f138f-361">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-362">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-362">Monitor</span></span>
* <span data-ttu-id="f138f-363">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="f138f-363">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="f138f-364">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-364">Network</span></span>
* <span data-ttu-id="f138f-365">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-365">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="f138f-366">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-366">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="f138f-367">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-367">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="f138f-368">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="f138f-368">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="f138f-369">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="f138f-369">PrivateDNS</span></span>
* <span data-ttu-id="f138f-370">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-370">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-371">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-371">Resource</span></span>
* <span data-ttu-id="f138f-372">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-372">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="f138f-373">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-373">Role</span></span>
* <span data-ttu-id="f138f-374">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="f138f-374">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="f138f-375">[BREAKING CHANGE] `role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="f138f-375">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-376">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-376">SQL</span></span>
* <span data-ttu-id="f138f-377">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-377">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-378">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-378">Storage</span></span>
* <span data-ttu-id="f138f-379">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-379">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="f138f-380">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f138f-380">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="f138f-381">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="f138f-381">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="f138f-382">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-382">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="f138f-383">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-383">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="f138f-384">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-384">Core</span></span>
* <span data-ttu-id="f138f-385">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-385">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="f138f-386">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="f138f-386">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="f138f-387">Cloud</span><span class="sxs-lookup"><span data-stu-id="f138f-387">Cloud</span></span>
* <span data-ttu-id="f138f-388">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-388">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-389">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-389">ACR</span></span>
* <span data-ttu-id="f138f-390">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-390">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="f138f-391">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-391">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="f138f-392">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-392">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="f138f-393">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-393">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-394">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-394">AppService</span></span>
* <span data-ttu-id="f138f-395">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-395">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="f138f-396">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-396">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="f138f-397">Bot Service</span><span class="sxs-lookup"><span data-stu-id="f138f-397">BOT Service</span></span>
* <span data-ttu-id="f138f-398">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="f138f-398">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="f138f-399">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-399">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="f138f-400">[BREAKING CHANGE] `--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="f138f-400">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="f138f-401">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-401">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-402">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-402">CDN</span></span>
* <span data-ttu-id="f138f-403">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-403">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="f138f-404">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="f138f-404">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="f138f-405">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f138f-405">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f138f-406">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f138f-406">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-407">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f138f-407">Cosmosdb</span></span>
* <span data-ttu-id="f138f-408">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-408">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="f138f-409">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-409">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-410">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-410">Interactive</span></span>
* <span data-ttu-id="f138f-411">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-411">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-412">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-412">Monitor</span></span>
* <span data-ttu-id="f138f-413">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f138f-413">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-414">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-414">Network</span></span>
* <span data-ttu-id="f138f-415">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-415">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-416">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-416">Profile</span></span>
* <span data-ttu-id="f138f-417">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-417">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="f138f-418">Postgres</span><span class="sxs-lookup"><span data-stu-id="f138f-418">Postgres</span></span> 
* <span data-ttu-id="f138f-419">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-419">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="f138f-420">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f138f-420">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-421">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-421">Resource</span></span>
* <span data-ttu-id="f138f-422">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f138f-422">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="f138f-423">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-423">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="f138f-424">Graph</span><span class="sxs-lookup"><span data-stu-id="f138f-424">Graph</span></span>
* <span data-ttu-id="f138f-425">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-425">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="f138f-426">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-426">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="f138f-427">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="f138f-427">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="f138f-428">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="f138f-428">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="f138f-429">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-429">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-430">storage</span><span class="sxs-lookup"><span data-stu-id="f138f-430">storage</span></span>
* <span data-ttu-id="f138f-431">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-431">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="f138f-432">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="f138f-432">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="f138f-433">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-433">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="f138f-434">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-434">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-435">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-435">VM</span></span>
* <span data-ttu-id="f138f-436">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-436">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="f138f-437">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-437">March 12, 2019</span></span>

<span data-ttu-id="f138f-438">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="f138f-438">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="f138f-439">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-439">Core</span></span>

* <span data-ttu-id="f138f-440">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-440">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-441">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-441">ACR</span></span>

* <span data-ttu-id="f138f-442">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-442">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-443">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-443">ACS</span></span>

* <span data-ttu-id="f138f-444">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-444">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="f138f-445">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-445">AppService</span></span>

* <span data-ttu-id="f138f-446">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="f138f-446">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="f138f-447">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-447">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="f138f-448">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="f138f-448">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="f138f-449">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="f138f-449">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-450">Botservice</span><span class="sxs-lookup"><span data-stu-id="f138f-450">Botservice</span></span>

* <span data-ttu-id="f138f-451">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-451">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f138f-452">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-452">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f138f-453">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-453">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="f138f-454">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="f138f-454">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="f138f-455">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-455">Container</span></span>

* <span data-ttu-id="f138f-456">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-456">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="f138f-457">EventHub</span><span class="sxs-lookup"><span data-stu-id="f138f-457">EventHub</span></span>

* <span data-ttu-id="f138f-458">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-458">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="f138f-459">Suchen</span><span class="sxs-lookup"><span data-stu-id="f138f-459">Find</span></span>

* <span data-ttu-id="f138f-460">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="f138f-460">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f138f-461">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f138f-461">HDInsight</span></span>

* <span data-ttu-id="f138f-462">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-462">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="f138f-463">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-463">Network</span></span>

* <span data-ttu-id="f138f-464">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="f138f-464">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-465">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f138f-465">Rdbms</span></span>

* <span data-ttu-id="f138f-466">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f138f-466">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="f138f-467">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-467">Role</span></span>

* <span data-ttu-id="f138f-468">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="f138f-468">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="f138f-469">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f138f-469">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f138f-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f138f-470">Service Fabric</span></span>

* <span data-ttu-id="f138f-471">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-471">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="f138f-472">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-472">February 26, 2019</span></span>

<span data-ttu-id="f138f-473">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="f138f-473">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="f138f-474">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-474">Core</span></span>

* <span data-ttu-id="f138f-475">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="f138f-475">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-476">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-476">ACR</span></span>

* <span data-ttu-id="f138f-477">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-477">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="f138f-478">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="f138f-478">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-479">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-479">ACS</span></span>

* <span data-ttu-id="f138f-480">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-480">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-481">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-481">AppService</span></span>

* <span data-ttu-id="f138f-482">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-482">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-483">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-483">Batch</span></span>
* <span data-ttu-id="f138f-484">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-484">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="f138f-485">[BREAKING CHANGE] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-485">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="f138f-486">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-486">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="f138f-487">[BREAKING CHANGE] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-487">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="f138f-488">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-488">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="f138f-489">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="f138f-489">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-490">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-490">CosmosDB</span></span>

* <span data-ttu-id="f138f-491">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-491">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="f138f-492">Kusto</span><span class="sxs-lookup"><span data-stu-id="f138f-492">Kusto</span></span>

* <span data-ttu-id="f138f-493">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-493">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="f138f-494">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-494">Network</span></span>

* <span data-ttu-id="f138f-495">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-495">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="f138f-496">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-496">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="f138f-497">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-497">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="f138f-498">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-498">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="f138f-499">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-499">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="f138f-500">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-500">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="f138f-501">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-501">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-502">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-502">Resource</span></span>

* <span data-ttu-id="f138f-503">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-503">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="f138f-504">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-504">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="f138f-505">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-505">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="f138f-506">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-506">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="f138f-507">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-507">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="f138f-508">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-508">Role</span></span>

* <span data-ttu-id="f138f-509">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-509">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-510">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-510">VM</span></span>

* <span data-ttu-id="f138f-511">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="f138f-511">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="f138f-512">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-512">February 12, 2019</span></span>

<span data-ttu-id="f138f-513">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="f138f-513">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="f138f-514">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-514">Core</span></span>

* <span data-ttu-id="f138f-515">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-515">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="f138f-516">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-516">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-517">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-517">ACR</span></span>
* <span data-ttu-id="f138f-518">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-518">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="f138f-519">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-519">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-520">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-520">ACS</span></span>
* <span data-ttu-id="f138f-521">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-521">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="f138f-522">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-522">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="f138f-523">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-523">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-524">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-524">AMS</span></span>
* <span data-ttu-id="f138f-525">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-525">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="f138f-526">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-526">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-527">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-527">Appservice</span></span>
* <span data-ttu-id="f138f-528">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-528">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="f138f-529">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-529">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="f138f-530">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f138f-530">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="f138f-531">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-531">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="f138f-532">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-532">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-533">Botservice</span><span class="sxs-lookup"><span data-stu-id="f138f-533">Botservice</span></span>
* <span data-ttu-id="f138f-534">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f138f-534">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="f138f-535">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-535">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="f138f-536">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-536">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="f138f-537">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="f138f-537">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="f138f-538">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-538">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="f138f-539">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="f138f-539">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="f138f-540">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-540">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="f138f-541">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-541">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="f138f-542">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="f138f-542">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="f138f-543">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="f138f-543">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="f138f-544">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f138f-544">Key Vault</span></span>
* <span data-ttu-id="f138f-545">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="f138f-545">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-546">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-546">Monitor</span></span>
* <span data-ttu-id="f138f-547">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-547">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-548">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-548">Network</span></span>
* <span data-ttu-id="f138f-549">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="f138f-549">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="f138f-550">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f138f-550">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="f138f-551">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f138f-551">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="f138f-552">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-552">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f138f-553">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f138f-553">Policy Insights</span></span>
* <span data-ttu-id="f138f-554">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f138f-554">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-555">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-555">RDBMS</span></span>
* <span data-ttu-id="f138f-556">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="f138f-556">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="f138f-557">Redis</span><span class="sxs-lookup"><span data-stu-id="f138f-557">Redis</span></span>
* <span data-ttu-id="f138f-558">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-558">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="f138f-559">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-559">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="f138f-560">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-560">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="f138f-561">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-561">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="f138f-562">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-562">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="f138f-563">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-563">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="f138f-564">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-564">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="f138f-565">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-565">Role</span></span>
* <span data-ttu-id="f138f-566">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-566">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="f138f-567">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="f138f-567">SQL VM</span></span>
* <span data-ttu-id="f138f-568">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-568">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-569">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-569">VM</span></span>
* <span data-ttu-id="f138f-570">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="f138f-570">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="f138f-571">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-571">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="f138f-572">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="f138f-572">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="f138f-573">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-573">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="f138f-574">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-574">January 31, 2019</span></span>

<span data-ttu-id="f138f-575">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="f138f-575">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="f138f-576">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-576">Core</span></span>

* <span data-ttu-id="f138f-577">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="f138f-577">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="f138f-578">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-578">January 28, 2019</span></span>

<span data-ttu-id="f138f-579">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="f138f-579">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-580">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-580">ACR</span></span>
* <span data-ttu-id="f138f-581">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-581">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-582">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-582">ACS</span></span>
* <span data-ttu-id="f138f-583">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-583">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f138f-584">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-584">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="f138f-585">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-585">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-586">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-586">AMS</span></span>
* <span data-ttu-id="f138f-587">[BREAKING CHANGE] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-587">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="f138f-588">[BREAKING CHANGE] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-588">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-589">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-589">Appservice</span></span>
* <span data-ttu-id="f138f-590">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-590">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="f138f-591">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-591">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="f138f-592">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-592">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="f138f-593">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-593">Container</span></span>
* <span data-ttu-id="f138f-594">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-594">Added `container start` command</span></span>
* <span data-ttu-id="f138f-595">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="f138f-595">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f138f-596">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f138f-596">EventGrid</span></span>
* <span data-ttu-id="f138f-597">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-597">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="f138f-598">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-598">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="f138f-599">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-599">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="f138f-600">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-600">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="f138f-601">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-601">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f138f-602">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f138f-602">HDInsight</span></span>
* <span data-ttu-id="f138f-603">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-603">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="f138f-604">[BREAKING CHANGE] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-604">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="f138f-605">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-605">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="f138f-606">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-606">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="f138f-607">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-607">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="f138f-608">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-608">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-609">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-609">IoT</span></span>
* <span data-ttu-id="f138f-610">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-610">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="f138f-611">Kusto</span><span class="sxs-lookup"><span data-stu-id="f138f-611">Kusto</span></span>
* <span data-ttu-id="f138f-612">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f138f-612">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-613">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-613">Monitor</span></span>
* <span data-ttu-id="f138f-614">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-614">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-615">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-615">Profile</span></span>
* <span data-ttu-id="f138f-616">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f138f-616">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-617">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-617">Network</span></span>
* <span data-ttu-id="f138f-618">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="f138f-618">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="f138f-619">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="f138f-619">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-620">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-620">Resource</span></span>
* <span data-ttu-id="f138f-621">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-621">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="f138f-622">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-622">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="f138f-623">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="f138f-623">SQL Virtual Machine</span></span>
* <span data-ttu-id="f138f-624">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f138f-624">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-625">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-625">Storage</span></span>
* <span data-ttu-id="f138f-626">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-626">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="f138f-627">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-627">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-628">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-628">VM</span></span>
* <span data-ttu-id="f138f-629">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-629">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="f138f-630">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-630">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="f138f-631">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f138f-631">January 15, 2019</span></span>

<span data-ttu-id="f138f-632">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="f138f-632">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-633">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-633">ACR</span></span>
* <span data-ttu-id="f138f-634">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-634">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="f138f-635">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-635">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="f138f-636">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="f138f-636">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="f138f-637">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-637">ACS</span></span>
* <span data-ttu-id="f138f-638">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-638">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-639">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-639">Appservice</span></span>
* <span data-ttu-id="f138f-640">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="f138f-640">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="f138f-641">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-641">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="f138f-642">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-642">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="f138f-643">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-643">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-644">Botservice</span><span class="sxs-lookup"><span data-stu-id="f138f-644">Botservice</span></span>
* <span data-ttu-id="f138f-645">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-645">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="f138f-646">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f138f-646">Configure</span></span>
* <span data-ttu-id="f138f-647">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-647">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-648">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-648">CosmosDB</span></span>
* <span data-ttu-id="f138f-649">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-649">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f138f-650">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f138f-650">HDInsight</span></span>
* <span data-ttu-id="f138f-651">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-651">Added commands for managing applications</span></span>
* <span data-ttu-id="f138f-652">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-652">Added commands for managing script actions</span></span>
* <span data-ttu-id="f138f-653">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-653">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="f138f-654">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-654">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="f138f-655">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-655">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-656">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-656">Network</span></span>
* <span data-ttu-id="f138f-657">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-657">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="f138f-658">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="f138f-658">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="f138f-659">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-659">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="f138f-660">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="f138f-660">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="f138f-661">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-661">Role</span></span>
* <span data-ttu-id="f138f-662">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f138f-662">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="f138f-663">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="f138f-663">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="f138f-664">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="f138f-664">Security</span></span>
* <span data-ttu-id="f138f-665">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-665">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-666">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-666">Storage</span></span>
* <span data-ttu-id="f138f-667">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="f138f-667">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="f138f-668">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-668">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="f138f-669">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-669">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="f138f-670">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-670">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="f138f-671">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-671">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-672">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-672">VM</span></span>
* <span data-ttu-id="f138f-673">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="f138f-673">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="f138f-674">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-674">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f138f-675">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-675">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="f138f-676">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f138f-676">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="f138f-677">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="f138f-677">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="f138f-678">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="f138f-678">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="f138f-679">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-679">December 20, 2018</span></span>

<span data-ttu-id="f138f-680">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="f138f-680">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="f138f-681">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-681">Appservice</span></span>
* <span data-ttu-id="f138f-682">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-682">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="f138f-683">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-683">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="f138f-684">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-684">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f138f-685">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="f138f-685">IoTCentral</span></span>
* <span data-ttu-id="f138f-686">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-686">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="f138f-687">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-687">Role</span></span>
* <span data-ttu-id="f138f-688">[BREAKING CHANGE] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="f138f-688">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-689">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-689">SQL</span></span>
* <span data-ttu-id="f138f-690">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-690">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-691">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-691">VM</span></span>
* <span data-ttu-id="f138f-692">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-692">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="f138f-693">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-693">December 18, 2018</span></span>

<span data-ttu-id="f138f-694">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="f138f-694">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="f138f-695">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-695">ACR</span></span>
* <span data-ttu-id="f138f-696">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-696">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="f138f-697">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="f138f-697">Condensed the table layout for task list</span></span>
* <span data-ttu-id="f138f-698">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-698">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-699">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-699">ACS</span></span>
* <span data-ttu-id="f138f-700">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-700">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f138f-701">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-701">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="f138f-702">[VERALTET] `az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-702">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="f138f-703">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="f138f-703">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="f138f-704">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-704">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="f138f-705">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-705">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-706">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-706">Appservice</span></span>
* <span data-ttu-id="f138f-707">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-707">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="f138f-708">Botservice</span><span class="sxs-lookup"><span data-stu-id="f138f-708">Botservice</span></span>
* <span data-ttu-id="f138f-709">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-709">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="f138f-710">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-710">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="f138f-711">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-711">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="f138f-712">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="f138f-712">Reduced Kudu network calls</span></span>
* <span data-ttu-id="f138f-713">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f138f-713">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-714">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-714">Consumption</span></span>
* <span data-ttu-id="f138f-715">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-715">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-716">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-716">CosmosDB</span></span>
* <span data-ttu-id="f138f-717">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-717">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="f138f-718">Karten</span><span class="sxs-lookup"><span data-stu-id="f138f-718">Maps</span></span>
* <span data-ttu-id="f138f-719">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-719">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-720">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-720">Network</span></span>
* <span data-ttu-id="f138f-721">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-721">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="f138f-722">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f138f-722">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-723">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-723">Resource</span></span>
* <span data-ttu-id="f138f-724">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-724">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="f138f-725">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-725">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-726">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-726">Storage</span></span>
*  <span data-ttu-id="f138f-727">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-727">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-728">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-728">VM</span></span>
* <span data-ttu-id="f138f-729">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="f138f-729">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="f138f-730">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-730">December 4, 2018</span></span>

<span data-ttu-id="f138f-731">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="f138f-731">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="f138f-732">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-732">Core</span></span>
* <span data-ttu-id="f138f-733">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-733">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="f138f-734">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-734">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-735">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-735">Appservice</span></span>
* <span data-ttu-id="f138f-736">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="f138f-736">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="f138f-737">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-737">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="f138f-738">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-738">Network</span></span>
* <span data-ttu-id="f138f-739">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-739">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="f138f-740">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-740">Role</span></span>
* <span data-ttu-id="f138f-741">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-741">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="f138f-742">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-742">VM</span></span>
* <span data-ttu-id="f138f-743">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-743">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="f138f-744">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="f138f-744">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="f138f-745">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f138f-745">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="f138f-746">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="f138f-746">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="f138f-747">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-747">November 20, 2018</span></span>

<span data-ttu-id="f138f-748">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="f138f-748">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="f138f-749">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-749">Core</span></span>
* <span data-ttu-id="f138f-750">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-750">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-751">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-751">ACR</span></span>
* <span data-ttu-id="f138f-752">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-752">Added context token to task step</span></span>
* <span data-ttu-id="f138f-753">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-753">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="f138f-754">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-754">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-755">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-755">Appservice</span></span>
* <span data-ttu-id="f138f-756">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-756">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="f138f-757">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="f138f-757">Updated the default `node_version`.</span></span> <span data-ttu-id="f138f-758">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="f138f-758">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="f138f-759">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-759">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="f138f-760">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="f138f-760">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f138f-761">IotCentral</span><span class="sxs-lookup"><span data-stu-id="f138f-761">IotCentral</span></span>
* <span data-ttu-id="f138f-762">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-762">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-763">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-763">KeyVault</span></span>
* <span data-ttu-id="f138f-764">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-764">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="f138f-765">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-765">Network</span></span>
* <span data-ttu-id="f138f-766">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-766">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="f138f-767">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-767">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="f138f-768">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-768">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="f138f-769">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-769">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-770">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f138f-770">Rdbms</span></span>
* <span data-ttu-id="f138f-771">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-771">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="f138f-772">RBAC</span><span class="sxs-lookup"><span data-stu-id="f138f-772">Rbac</span></span>
* <span data-ttu-id="f138f-773">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-773">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="f138f-774">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-774">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="f138f-775">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-775">Storage</span></span>
* <span data-ttu-id="f138f-776">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-776">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="f138f-777">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="f138f-777">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="f138f-778">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-778">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="f138f-779">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-779">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-780">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-780">VM</span></span>
* <span data-ttu-id="f138f-781">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-781">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="f138f-782">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-782">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="f138f-783">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f138f-783">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="f138f-784">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-784">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="f138f-785">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-785">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="f138f-786">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-786">Added `snapshot wait` command</span></span>
* <span data-ttu-id="f138f-787">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-787">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f138f-788">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-788">November 6, 2018</span></span>

<span data-ttu-id="f138f-789">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f138f-789">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f138f-790">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-790">Core</span></span>
* <span data-ttu-id="f138f-791">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-791">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-792">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-792">ACR</span></span>
* <span data-ttu-id="f138f-793">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-793">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f138f-794">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-794">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-795">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-795">ACS</span></span>
* <span data-ttu-id="f138f-796">[BREAKING CHANGE] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="f138f-796">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f138f-797">Advisor</span><span class="sxs-lookup"><span data-stu-id="f138f-797">Advisor</span></span>
* <span data-ttu-id="f138f-798">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="f138f-798">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-799">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-799">AMS</span></span>
* <span data-ttu-id="f138f-800">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-800">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f138f-801">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-801">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f138f-802">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-802">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f138f-803">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-803">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f138f-804">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-804">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f138f-805">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-805">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f138f-806">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-806">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f138f-807">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f138f-807">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f138f-808">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-808">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f138f-809">[BREAKING CHANGE] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-809">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f138f-810">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f138f-810">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f138f-811">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f138f-811">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f138f-812">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="f138f-812">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f138f-813">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-813">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f138f-814">[BREAKING CHANGE] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f138f-814">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f138f-815">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-815">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f138f-816">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="f138f-816">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-817">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-817">AppService</span></span>
* <span data-ttu-id="f138f-818">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="f138f-818">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f138f-819">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f138f-819">Configure</span></span>
* <span data-ttu-id="f138f-820">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-820">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f138f-821">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-821">Container</span></span>
* <span data-ttu-id="f138f-822">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="f138f-822">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f138f-823">EventHub</span><span class="sxs-lookup"><span data-stu-id="f138f-823">EventHub</span></span>
* <span data-ttu-id="f138f-824">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-824">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-825">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-825">Interactive</span></span>
* <span data-ttu-id="f138f-826">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-826">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-827">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-827">Monitor</span></span>
* <span data-ttu-id="f138f-828">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-828">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-829">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-829">Network</span></span>
* <span data-ttu-id="f138f-830">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-830">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f138f-831">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f138f-831">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f138f-832">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="f138f-832">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f138f-833">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-833">Profile</span></span>
* <span data-ttu-id="f138f-834">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-834">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-835">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-835">RDBMS</span></span>
* <span data-ttu-id="f138f-836">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-836">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-837">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-837">Resource</span></span>
* <span data-ttu-id="f138f-838">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-838">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f138f-839">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-839">Role</span></span>
* <span data-ttu-id="f138f-840">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-840">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f138f-841">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="f138f-841">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f138f-842">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-842">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-843">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-843">Storage</span></span>
* <span data-ttu-id="f138f-844">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="f138f-844">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-845">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-845">VM</span></span>
* <span data-ttu-id="f138f-846">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-846">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f138f-847">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="f138f-847">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f138f-848">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-848">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f138f-849">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="f138f-849">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f138f-850">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-850">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f138f-851">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-851">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f138f-852">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-852">October 23, 2018</span></span>

<span data-ttu-id="f138f-853">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f138f-853">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f138f-854">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-854">Core</span></span>
* <span data-ttu-id="f138f-855">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="f138f-855">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f138f-856">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="f138f-856">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-857">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-857">ACR</span></span>
* <span data-ttu-id="f138f-858">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-858">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-859">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-859">CDN</span></span>
* <span data-ttu-id="f138f-860">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-860">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f138f-861">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f138f-861">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f138f-862">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-862">Container</span></span>
* <span data-ttu-id="f138f-863">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-863">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f138f-864">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f138f-864">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f138f-865">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-865">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f138f-866">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f138f-866">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f138f-867">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f138f-867">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f138f-868">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-868">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f138f-869">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-869">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-870">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-870">CosmosDB</span></span>
* <span data-ttu-id="f138f-871">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-871">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-872">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-872">Interactive</span></span>
* <span data-ttu-id="f138f-873">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-873">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f138f-874">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f138f-874">IoT Central</span></span>
* <span data-ttu-id="f138f-875">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-875">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f138f-876">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f138f-876">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-877">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-877">Monitor</span></span>
* <span data-ttu-id="f138f-878">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="f138f-878">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f138f-879">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-879">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f138f-880">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-880">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f138f-881">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-881">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f138f-882">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-882">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f138f-883">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-883">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f138f-884">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="f138f-884">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f138f-885">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-885">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f138f-886">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-886">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f138f-887">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-887">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-888">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-888">Network</span></span>
* <span data-ttu-id="f138f-889">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-889">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f138f-890">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-890">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f138f-891">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f138f-891">ServiceBus</span></span>
* <span data-ttu-id="f138f-892">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-892">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-893">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-893">SQL</span></span>
* <span data-ttu-id="f138f-894">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="f138f-894">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-895">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-895">Storage</span></span>
* <span data-ttu-id="f138f-896">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-896">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f138f-897">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-897">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-898">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-898">VM</span></span>
* <span data-ttu-id="f138f-899">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="f138f-899">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f138f-900">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-900">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f138f-901">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-901">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f138f-902">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-902">October 16, 2018</span></span>

<span data-ttu-id="f138f-903">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f138f-903">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-904">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-904">VM</span></span>
* <span data-ttu-id="f138f-905">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="f138f-905">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f138f-906">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-906">October 9, 2018</span></span>

<span data-ttu-id="f138f-907">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f138f-907">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f138f-908">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-908">Core</span></span>
* <span data-ttu-id="f138f-909">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="f138f-909">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-910">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-910">ACR</span></span>
* <span data-ttu-id="f138f-911">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-911">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-912">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-912">ACS</span></span>
* <span data-ttu-id="f138f-913">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="f138f-913">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f138f-914">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="f138f-914">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f138f-915">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f138f-915">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f138f-916">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="f138f-916">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f138f-917">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-917">Container</span></span>
* <span data-ttu-id="f138f-918">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-918">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f138f-919">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-919">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f138f-920">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f138f-920">Event Hub</span></span>
* <span data-ttu-id="f138f-921">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-921">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f138f-922">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-922">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f138f-923">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f138f-923">Extensions</span></span>
* <span data-ttu-id="f138f-924">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="f138f-924">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f138f-925">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f138f-925">HDInsight</span></span>
* <span data-ttu-id="f138f-926">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-926">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-927">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-927">IoT</span></span>
* <span data-ttu-id="f138f-928">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-928">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-929">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-929">KeyVault</span></span>
* <span data-ttu-id="f138f-930">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="f138f-930">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f138f-931">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-931">Network</span></span>
* <span data-ttu-id="f138f-932">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="f138f-932">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f138f-933">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="f138f-933">See #6052</span></span>
* <span data-ttu-id="f138f-934">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f138f-934">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f138f-935">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f138f-935">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f138f-936">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-936">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f138f-937">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-937">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f138f-938">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f138f-938">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f138f-939">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-939">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f138f-940">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-940">Role</span></span>
* <span data-ttu-id="f138f-941">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-941">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f138f-942">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-942">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f138f-943">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f138f-943">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f138f-944">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="f138f-944">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f138f-945">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f138f-945">Service Bus</span></span>
* <span data-ttu-id="f138f-946">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-946">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-947">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-947">VM</span></span>
* <span data-ttu-id="f138f-948">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-948">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f138f-949">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="f138f-949">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f138f-950">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-950">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f138f-951">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-951">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f138f-952">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-952">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f138f-953">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-953">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f138f-954">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-954">September 21, 2018</span></span>

<span data-ttu-id="f138f-955">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f138f-955">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-956">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-956">ACR</span></span>
* <span data-ttu-id="f138f-957">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-957">Added ACR Task commands</span></span>
* <span data-ttu-id="f138f-958">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-958">Added quick run command</span></span>
* <span data-ttu-id="f138f-959">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-959">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f138f-960">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-960">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f138f-961">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-961">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f138f-962">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-962">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-963">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-963">ACS</span></span>
* <span data-ttu-id="f138f-964">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-964">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f138f-965">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-965">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-966">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-966">AppService</span></span>

* <span data-ttu-id="f138f-967">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="f138f-967">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f138f-968">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-968">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f138f-969">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-969">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f138f-970">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-970">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-971">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-971">Batch</span></span>
* <span data-ttu-id="f138f-972">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-972">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f138f-973">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-973">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f138f-974">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-974">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f138f-975">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-975">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f138f-976">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f138f-976">Batch AI</span></span> 
* <span data-ttu-id="f138f-977">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-977">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f138f-978">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f138f-978">Cognitive Services</span></span>
* <span data-ttu-id="f138f-979">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-979">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f138f-980">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-980">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f138f-981">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-981">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f138f-982">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-982">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f138f-983">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-983">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f138f-984">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="f138f-984">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f138f-985">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-985">Container</span></span>
* <span data-ttu-id="f138f-986">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-986">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f138f-987">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-987">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f138f-988">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-988">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f138f-989">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-989">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f138f-990">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f138f-990">Datalake</span></span>
* <span data-ttu-id="f138f-991">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-991">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f138f-992">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="f138f-992">Interactive Shell</span></span>
* <span data-ttu-id="f138f-993">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-993">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f138f-994">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-994">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-995">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-995">IoT</span></span>
* <span data-ttu-id="f138f-996">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-996">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f138f-997">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f138f-997">Key Vault</span></span>
* <span data-ttu-id="f138f-998">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-998">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f138f-999">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-999">Network</span></span>
* <span data-ttu-id="f138f-1000">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-1000">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f138f-1001">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-1001">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f138f-1002">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-1002">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f138f-1003">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-1003">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f138f-1004">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1004">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f138f-1005">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1005">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f138f-1006">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-1006">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f138f-1007">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f138f-1007">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f138f-1008">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1008">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f138f-1009">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1009">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f138f-1010">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1010">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f138f-1011">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1011">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f138f-1012">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1012">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f138f-1013">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="f138f-1013">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f138f-1014">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1014">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f138f-1015">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="f138f-1015">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f138f-1016">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1016">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f138f-1017">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1017">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-1018">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1018">RDBMS</span></span>
* <span data-ttu-id="f138f-1019">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1019">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f138f-1020">Reservierung</span><span class="sxs-lookup"><span data-stu-id="f138f-1020">Reservation</span></span>
* <span data-ttu-id="f138f-1021">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1021">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f138f-1022">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1022">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f138f-1023">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="f138f-1023">Manage App</span></span>
* <span data-ttu-id="f138f-1024">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="f138f-1024">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f138f-1025">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="f138f-1025">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1026">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1026">Role</span></span>
* <span data-ttu-id="f138f-1027">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1027">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f138f-1028">SignalR</span><span class="sxs-lookup"><span data-stu-id="f138f-1028">SignalR</span></span>
* <span data-ttu-id="f138f-1029">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1029">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1030">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1030">Storage</span></span>
* <span data-ttu-id="f138f-1031">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1031">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f138f-1032">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1032">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1033">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1033">VM</span></span>
* <span data-ttu-id="f138f-1034">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="f138f-1034">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f138f-1035">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1035">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f138f-1036">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1036">August 28, 2018</span></span>

<span data-ttu-id="f138f-1037">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f138f-1037">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1038">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1038">Core</span></span>

* <span data-ttu-id="f138f-1039">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-1039">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f138f-1040">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1040">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1041">ACR</span></span>

* <span data-ttu-id="f138f-1042">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1042">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f138f-1043">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="f138f-1043">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1044">ACS</span></span>

* <span data-ttu-id="f138f-1045">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1045">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f138f-1046">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="f138f-1046">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1047">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1047">AppService</span></span>

* <span data-ttu-id="f138f-1048">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1048">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f138f-1049">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1049">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f138f-1050">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1050">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f138f-1051">Backup</span><span class="sxs-lookup"><span data-stu-id="f138f-1051">Backup</span></span>

* <span data-ttu-id="f138f-1052">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1052">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f138f-1053">Botdienst</span><span class="sxs-lookup"><span data-stu-id="f138f-1053">Bot Service</span></span>

* <span data-ttu-id="f138f-1054">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="f138f-1054">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f138f-1055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f138f-1055">Cognitive Services</span></span>

* <span data-ttu-id="f138f-1056">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1056">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-1057">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1057">IoT</span></span>

* <span data-ttu-id="f138f-1058">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1058">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1059">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1059">Monitor</span></span>

* <span data-ttu-id="f138f-1060">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1060">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f138f-1061">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1061">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1062">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1062">Network</span></span>

* <span data-ttu-id="f138f-1063">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1063">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1064">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1064">Resource</span></span>

* <span data-ttu-id="f138f-1065">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1065">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1066">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1066">Storage</span></span>

* <span data-ttu-id="f138f-1067">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1067">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1068">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1068">VM</span></span>

* <span data-ttu-id="f138f-1069">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f138f-1069">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f138f-1070">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f138f-1070">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f138f-1071">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1071">Auguest 14, 2018</span></span>

<span data-ttu-id="f138f-1072">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f138f-1072">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1073">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1073">Core</span></span>

* <span data-ttu-id="f138f-1074">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1074">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f138f-1075">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1075">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f138f-1076">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f138f-1076">Telemetry</span></span>

* <span data-ttu-id="f138f-1077">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="f138f-1077">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1078">ACR</span></span>

* <span data-ttu-id="f138f-1079">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1079">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f138f-1080">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-1080">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1081">ACS</span></span>

* <span data-ttu-id="f138f-1082">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1082">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f138f-1083">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f138f-1083">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f138f-1084">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="f138f-1084">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f138f-1085">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1085">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f138f-1086">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1086">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f138f-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1087">AppService</span></span>

* <span data-ttu-id="f138f-1088">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="f138f-1088">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f138f-1089">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1089">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-1090">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f138f-1090">BatchAI</span></span>

* <span data-ttu-id="f138f-1091">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1091">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="f138f-1092">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1092">Container</span></span>

* <span data-ttu-id="f138f-1093">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1093">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f138f-1094">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1094">IoT</span></span>

* <span data-ttu-id="f138f-1095">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1095">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f138f-1096">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="f138f-1096">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f138f-1097">Iot Central</span><span class="sxs-lookup"><span data-stu-id="f138f-1097">Iot Central</span></span>

* <span data-ttu-id="f138f-1098">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-1098">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-1099">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-1099">KeyVault</span></span>


* <span data-ttu-id="f138f-1100">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1100">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f138f-1101">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1101">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f138f-1102">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1102">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f138f-1103">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1103">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f138f-1104">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1104">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f138f-1105">Relay</span><span class="sxs-lookup"><span data-stu-id="f138f-1105">Relay</span></span>

* <span data-ttu-id="f138f-1106">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1106">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1107">Sql</span><span class="sxs-lookup"><span data-stu-id="f138f-1107">Sql</span></span>

* <span data-ttu-id="f138f-1108">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1108">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1109">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1109">Storage</span></span>

* <span data-ttu-id="f138f-1110">[BREAKING CHANGE] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="f138f-1110">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f138f-1111">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1111">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f138f-1112">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1112">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f138f-1113">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1113">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f138f-1114">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="f138f-1114">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1115">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1115">VM</span></span>

* <span data-ttu-id="f138f-1116">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1116">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f138f-1117">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1117">July 31, 2018</span></span>

<span data-ttu-id="f138f-1118">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f138f-1118">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1119">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1119">ACR</span></span>

* <span data-ttu-id="f138f-1120">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1120">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f138f-1121">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1121">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1122">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1122">ACS</span></span>

* <span data-ttu-id="f138f-1123">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1123">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1124">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1124">Batch</span></span>

* <span data-ttu-id="f138f-1125">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f138f-1125">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1126">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1126">Container</span></span>

* <span data-ttu-id="f138f-1127">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1127">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1128">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1128">Network</span></span>

* <span data-ttu-id="f138f-1129">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1129">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f138f-1130">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1130">Resource</span></span>

* <span data-ttu-id="f138f-1131">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f138f-1131">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f138f-1132">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="f138f-1132">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1133">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1133">Role</span></span>

* <span data-ttu-id="f138f-1134">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1134">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f138f-1135">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f138f-1135">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f138f-1136">Suchen,</span><span class="sxs-lookup"><span data-stu-id="f138f-1136">Search</span></span>

* <span data-ttu-id="f138f-1137">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1137">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f138f-1138">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f138f-1138">Service Bus</span></span>

* <span data-ttu-id="f138f-1139">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="f138f-1139">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f138f-1140">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1140">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f138f-1141">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="f138f-1141">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f138f-1142">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="f138f-1142">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1143">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1143">Storage</span></span>

* <span data-ttu-id="f138f-1144">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1144">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f138f-1145">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-1145">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1146">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1146">VM</span></span>

* <span data-ttu-id="f138f-1147">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1147">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f138f-1148">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1148">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f138f-1149">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1149">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f138f-1150">[BREAKING CHANGE] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-1150">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f138f-1151">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1151">July 18, 2018</span></span>

<span data-ttu-id="f138f-1152">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f138f-1152">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1153">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1153">Core</span></span>

* <span data-ttu-id="f138f-1154">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1154">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f138f-1155">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1155">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f138f-1156">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="f138f-1156">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1157">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1157">ACR</span></span>

* <span data-ttu-id="f138f-1158">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1158">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f138f-1159">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1159">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f138f-1160">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-1160">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f138f-1161">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1161">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1162">ACS</span></span>

* <span data-ttu-id="f138f-1163">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1163">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1164">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1164">AppService</span></span>

* <span data-ttu-id="f138f-1165">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1165">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1166">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1166">Batch</span></span>

* <span data-ttu-id="f138f-1167">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="f138f-1167">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f138f-1168">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1168">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f138f-1169">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f138f-1169">Batch AI</span></span>

* <span data-ttu-id="f138f-1170">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1170">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1171">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1171">Container</span></span>

* <span data-ttu-id="f138f-1172">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1172">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f138f-1173">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1173">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1174">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1174">Network</span></span>

* <span data-ttu-id="f138f-1175">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1175">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f138f-1176">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1176">Added `network nic wait`</span></span>
* <span data-ttu-id="f138f-1177">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1177">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f138f-1178">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="f138f-1178">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f138f-1179">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1179">Resource</span></span>

* <span data-ttu-id="f138f-1180">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1180">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f138f-1181">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1181">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f138f-1182">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1182">Added `deployment wait` command</span></span>
* <span data-ttu-id="f138f-1183">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1183">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1184">SQL</span></span>

* <span data-ttu-id="f138f-1185">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1185">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f138f-1186">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="f138f-1186">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f138f-1187">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1187">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1188">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1188">Storage</span></span>

* <span data-ttu-id="f138f-1189">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1189">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1190">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1190">VM</span></span>

* <span data-ttu-id="f138f-1191">[BREAKING CHANGE] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1191">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f138f-1192">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1192">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f138f-1193">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1193">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f138f-1194">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1194">July 3, 2018</span></span>

<span data-ttu-id="f138f-1195">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f138f-1195">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f138f-1196">AKS</span><span class="sxs-lookup"><span data-stu-id="f138f-1196">AKS</span></span>

* <span data-ttu-id="f138f-1197">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1197">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f138f-1198">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1198">July 3, 2018</span></span>

<span data-ttu-id="f138f-1199">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f138f-1199">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1200">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1200">Core</span></span>

* <span data-ttu-id="f138f-1201">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1201">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1202">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1202">ACR</span></span>

* <span data-ttu-id="f138f-1203">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1203">Added polling build status</span></span>
* <span data-ttu-id="f138f-1204">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1204">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f138f-1205">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1205">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1206">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1206">ACS</span></span>

* <span data-ttu-id="f138f-1207">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f138f-1207">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f138f-1208">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1208">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f138f-1209">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1209">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f138f-1210">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1210">Added `--listen-port` support</span></span>
* <span data-ttu-id="f138f-1211">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1211">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f138f-1212">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="f138f-1212">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f138f-1213">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1213">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1214">AppService</span></span>

* <span data-ttu-id="f138f-1215">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1215">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f138f-1216">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1216">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f138f-1217">Backup</span><span class="sxs-lookup"><span data-stu-id="f138f-1217">Backup</span></span>

* <span data-ttu-id="f138f-1218">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1218">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-1219">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f138f-1219">BatchAI</span></span>

* <span data-ttu-id="f138f-1220">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1220">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f138f-1221">Cloud</span><span class="sxs-lookup"><span data-stu-id="f138f-1221">Cloud</span></span>

* <span data-ttu-id="f138f-1222">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1222">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1223">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1223">Container</span></span>

* <span data-ttu-id="f138f-1224">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1224">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f138f-1225">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1225">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f138f-1226">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1226">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1227">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1227">Extension</span></span>

* <span data-ttu-id="f138f-1228">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1228">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1229">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1229">Network</span></span>

* <span data-ttu-id="f138f-1230">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f138f-1230">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-1231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f138f-1231">Rdbms</span></span>

* <span data-ttu-id="f138f-1232">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1232">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1233">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1233">Resource</span></span>

* <span data-ttu-id="f138f-1234">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1234">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1235">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1235">VM</span></span>

* <span data-ttu-id="f138f-1236">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1236">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f138f-1237">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1237">June 25, 2018</span></span>

<span data-ttu-id="f138f-1238">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f138f-1238">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f138f-1239">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f138f-1239">CLI</span></span>

* <span data-ttu-id="f138f-1240">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="f138f-1240">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f138f-1241">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1241">June 19, 2018</span></span>

<span data-ttu-id="f138f-1242">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f138f-1242">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1243">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1243">Core</span></span>

* <span data-ttu-id="f138f-1244">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1244">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1245">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1245">ACR</span></span>

* <span data-ttu-id="f138f-1246">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1246">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f138f-1247">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1247">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1248">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1248">ACS</span></span>

* <span data-ttu-id="f138f-1249">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1249">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f138f-1250">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1250">Added `--update` support</span></span>
* <span data-ttu-id="f138f-1251">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1251">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f138f-1252">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-1252">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f138f-1253">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1253">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f138f-1254">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="f138f-1254">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f138f-1255">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1255">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f138f-1256">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1256">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1257">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1257">AppService</span></span>

* <span data-ttu-id="f138f-1258">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1258">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f138f-1259">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1259">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1260">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1260">Batch</span></span>

* <span data-ttu-id="f138f-1261">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1261">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f138f-1262">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f138f-1262">Batch AI</span></span>

* <span data-ttu-id="f138f-1263">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1263">Added support for workspaces.</span></span> <span data-ttu-id="f138f-1264">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="f138f-1264">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f138f-1265">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1265">Added support for experiments.</span></span> <span data-ttu-id="f138f-1266">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="f138f-1266">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f138f-1267">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1267">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f138f-1268">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1268">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f138f-1269">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="f138f-1269">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f138f-1270">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1270">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f138f-1271">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-1271">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f138f-1272">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-1272">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f138f-1273">[BREAKING CHANGE] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1273">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f138f-1274">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="f138f-1274">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f138f-1275">[BREAKING CHANGE] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1275">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f138f-1276">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="f138f-1276">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f138f-1277">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1277">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f138f-1278">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="f138f-1278">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f138f-1279">[BREAKING CHANGE] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1279">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f138f-1280">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="f138f-1280">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f138f-1281">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1281">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f138f-1282">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1282">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f138f-1283">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1283">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f138f-1284">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1284">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f138f-1285">Karten</span><span class="sxs-lookup"><span data-stu-id="f138f-1285">Maps</span></span>

* <span data-ttu-id="f138f-1286">[BREAKING CHANGE] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f138f-1286">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1287">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1287">Network</span></span>

* <span data-ttu-id="f138f-1288">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="f138f-1288">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f138f-1289">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f138f-1289">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f138f-1290">#6502</span><span class="sxs-lookup"><span data-stu-id="f138f-1290">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f138f-1291">Reservations</span><span class="sxs-lookup"><span data-stu-id="f138f-1291">Reservations</span></span>

* <span data-ttu-id="f138f-1292">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1292">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f138f-1293">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1293">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f138f-1294">[BREAKING CHANGE] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1294">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f138f-1295">[BREAKING CHANGE] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1295">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f138f-1296">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1296">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f138f-1297">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1297">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1298">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1298">Role</span></span>

* <span data-ttu-id="f138f-1299">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1299">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1300">SQL</span></span>

* <span data-ttu-id="f138f-1301">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1301">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1302">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1302">Storage</span></span>

* <span data-ttu-id="f138f-1303">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1303">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1304">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1304">VM</span></span>

* <span data-ttu-id="f138f-1305">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="f138f-1305">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f138f-1306">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1306">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f138f-1307">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-1307">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f138f-1308">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1308">June 13, 2018</span></span>

<span data-ttu-id="f138f-1309">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f138f-1309">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1310">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1310">Core</span></span>

* <span data-ttu-id="f138f-1311">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f138f-1311">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f138f-1312">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1312">June 13, 2018</span></span>

<span data-ttu-id="f138f-1313">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f138f-1313">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f138f-1314">AKS</span><span class="sxs-lookup"><span data-stu-id="f138f-1314">AKS</span></span>

* <span data-ttu-id="f138f-1315">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1315">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f138f-1316">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1316">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f138f-1317">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1317">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f138f-1318">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1318">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f138f-1319">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1319">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1320">AppService</span></span>

* <span data-ttu-id="f138f-1321">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1321">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f138f-1322">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1322">June 5, 2018</span></span>

<span data-ttu-id="f138f-1323">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f138f-1323">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1324">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1324">Interactive</span></span>

* <span data-ttu-id="f138f-1325">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1325">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f138f-1326">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1326">June 5, 2018</span></span>

<span data-ttu-id="f138f-1327">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f138f-1327">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1328">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1328">Core</span></span>

* <span data-ttu-id="f138f-1329">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1329">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f138f-1330">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="f138f-1330">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1331">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1331">ACR</span></span>

* <span data-ttu-id="f138f-1332">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1332">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f138f-1333">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1333">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f138f-1334">AKS</span><span class="sxs-lookup"><span data-stu-id="f138f-1334">AKS</span></span>

* <span data-ttu-id="f138f-1335">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f138f-1335">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1336">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1336">Batch</span></span>

* <span data-ttu-id="f138f-1337">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f138f-1337">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-1338">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1338">IOT</span></span>

* <span data-ttu-id="f138f-1339">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1339">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1340">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1340">Network</span></span>

* <span data-ttu-id="f138f-1341">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1341">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f138f-1342">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f138f-1342">Policy Insights</span></span>

* <span data-ttu-id="f138f-1343">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1343">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f138f-1344">ARM</span><span class="sxs-lookup"><span data-stu-id="f138f-1344">ARM</span></span>

* <span data-ttu-id="f138f-1345">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1345">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1346">SQL</span></span>

* <span data-ttu-id="f138f-1347">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-1347">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f138f-1348">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-1348">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f138f-1349">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1349">Storage</span></span>

* <span data-ttu-id="f138f-1350">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="f138f-1350">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1351">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1351">VM</span></span>

* <span data-ttu-id="f138f-1352">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-1352">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f138f-1353">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1353">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f138f-1354">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1354">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f138f-1355">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1355">May 22, 2018</span></span>

<span data-ttu-id="f138f-1356">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f138f-1356">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1357">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1357">Core</span></span>

* <span data-ttu-id="f138f-1358">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1358">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1359">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1359">ACS</span></span>

* <span data-ttu-id="f138f-1360">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1360">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f138f-1361">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1361">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1362">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1362">AppService</span></span>

* <span data-ttu-id="f138f-1363">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="f138f-1363">Improved generic update commands</span></span>
* <span data-ttu-id="f138f-1364">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1364">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1365">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1365">Container</span></span>

* <span data-ttu-id="f138f-1366">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1366">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f138f-1367">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1367">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1368">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1368">Extension</span></span>

* <span data-ttu-id="f138f-1369">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f138f-1369">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1370">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1370">Interactive</span></span>

* <span data-ttu-id="f138f-1371">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="f138f-1371">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f138f-1372">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="f138f-1372">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-1373">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-1373">KeyVault</span></span>

* <span data-ttu-id="f138f-1374">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f138f-1374">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1375">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1375">Network</span></span>

* <span data-ttu-id="f138f-1376">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="f138f-1376">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f138f-1377">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="f138f-1377">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1378">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1378">SQL</span></span>

* <span data-ttu-id="f138f-1379">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="f138f-1379">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f138f-1380">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1380">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f138f-1381">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1381">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f138f-1382">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="f138f-1382">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f138f-1383">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f138f-1383">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f138f-1384">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1384">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f138f-1385">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="f138f-1385">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f138f-1386">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1386">`edition`.</span></span> <span data-ttu-id="f138f-1387">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="f138f-1387">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f138f-1388">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1388">`elasticPoolName`.</span></span> <span data-ttu-id="f138f-1389">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="f138f-1389">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f138f-1390">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f138f-1390">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f138f-1391">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1391">`edition`.</span></span> <span data-ttu-id="f138f-1392">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1392">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f138f-1393">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1393">`dtu`.</span></span> <span data-ttu-id="f138f-1394">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1394">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f138f-1395">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1395">`databaseDtuMin`.</span></span> <span data-ttu-id="f138f-1396">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1396">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f138f-1397">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1397">`databaseDtuMax`.</span></span> <span data-ttu-id="f138f-1398">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1398">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f138f-1399">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1399">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f138f-1400">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1400">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1401">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1401">Storage</span></span>

* <span data-ttu-id="f138f-1402">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1402">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f138f-1403">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1403">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1404">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1404">VM</span></span>

* <span data-ttu-id="f138f-1405">[BREAKING CHANGE] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1405">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f138f-1406">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-1406">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f138f-1407">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1407">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f138f-1408">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1408">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f138f-1409">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1409">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f138f-1410">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1410">May 7, 2018</span></span>

<span data-ttu-id="f138f-1411">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f138f-1411">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1412">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1412">Core</span></span>

* <span data-ttu-id="f138f-1413">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="f138f-1413">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f138f-1414">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1414">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f138f-1415">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-1415">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f138f-1416">#5591</span><span class="sxs-lookup"><span data-stu-id="f138f-1416">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f138f-1417">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1417">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f138f-1418">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="f138f-1418">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f138f-1419">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="f138f-1419">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f138f-1420">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="f138f-1420">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f138f-1421">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1421">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1422">ACR</span></span>

* <span data-ttu-id="f138f-1423">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1423">Added ACR Build commands</span></span>
* <span data-ttu-id="f138f-1424">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1424">Improved resource not found error messages</span></span>
* <span data-ttu-id="f138f-1425">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="f138f-1425">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f138f-1426">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1426">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f138f-1427">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1427">Improved repository commands error messages</span></span>
* <span data-ttu-id="f138f-1428">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1428">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1429">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1429">ACS</span></span>

* <span data-ttu-id="f138f-1430">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1430">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f138f-1431">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1431">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f138f-1432">AMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1432">AMS</span></span>

* <span data-ttu-id="f138f-1433">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f138f-1433">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1434">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1434">Appservice</span></span>

* <span data-ttu-id="f138f-1435">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="f138f-1435">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f138f-1436">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1436">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f138f-1437">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1437">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f138f-1438">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1438">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f138f-1439">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f138f-1439">Batch AI</span></span>

* <span data-ttu-id="f138f-1440">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="f138f-1440">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f138f-1441">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f138f-1441">Cognitive Services</span></span>

* <span data-ttu-id="f138f-1442">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="f138f-1442">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-1443">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-1443">Consumption</span></span>

* <span data-ttu-id="f138f-1444">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1444">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1445">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1445">Container</span></span>

* <span data-ttu-id="f138f-1446">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-1446">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f138f-1447">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f138f-1447">Cosmos DB</span></span>

* <span data-ttu-id="f138f-1448">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f138f-1448">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f138f-1449">DMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1449">DMS</span></span>

* <span data-ttu-id="f138f-1450">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1450">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1451">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1451">Extension</span></span>

* <span data-ttu-id="f138f-1452">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1452">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1453">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1453">Interactive</span></span>

* <span data-ttu-id="f138f-1454">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="f138f-1454">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f138f-1455">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="f138f-1455">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f138f-1456">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1456">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f138f-1457">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1457">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f138f-1458">Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-1458">Lab</span></span>

* <span data-ttu-id="f138f-1459">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1459">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1460">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1460">Network</span></span>

* <span data-ttu-id="f138f-1461">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="f138f-1461">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f138f-1462">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1462">Profile</span></span>

* <span data-ttu-id="f138f-1463">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1463">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f138f-1464">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1464">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f138f-1465">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1465">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f138f-1466">Redis</span><span class="sxs-lookup"><span data-stu-id="f138f-1466">Redis</span></span>

* <span data-ttu-id="f138f-1467">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1467">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f138f-1468">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1468">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f138f-1469">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1469">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f138f-1470">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1470">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f138f-1471">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1471">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1472">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1472">Role</span></span>

* <span data-ttu-id="f138f-1473">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1473">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1474">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1474">Storage</span></span>

* <span data-ttu-id="f138f-1475">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1475">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f138f-1476">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="f138f-1476">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f138f-1477">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="f138f-1477">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f138f-1478">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="f138f-1478">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f138f-1479">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f138f-1479">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1480">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1480">VM</span></span>

* <span data-ttu-id="f138f-1481">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1481">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f138f-1482">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1482">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f138f-1483">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="f138f-1483">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f138f-1484">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1484">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f138f-1485">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="f138f-1485">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f138f-1486">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1486">Added write accelerator support</span></span>
* <span data-ttu-id="f138f-1487">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1487">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f138f-1488">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="f138f-1488">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f138f-1489">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f138f-1489">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f138f-1490">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1490">April 10, 2018</span></span>

<span data-ttu-id="f138f-1491">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f138f-1491">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1492">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1492">ACR</span></span>

* <span data-ttu-id="f138f-1493">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="f138f-1493">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1494">ACS</span></span>

* <span data-ttu-id="f138f-1495">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1495">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1496">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1496">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f138f-1498">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1498">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-1499">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f138f-1499">BatchAI</span></span>

* <span data-ttu-id="f138f-1500">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1500">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f138f-1501">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="f138f-1501">Job level mounting</span></span>
  - <span data-ttu-id="f138f-1502">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="f138f-1502">Environment variables with secret values</span></span>
  - <span data-ttu-id="f138f-1503">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="f138f-1503">Performance counters settings</span></span>
  - <span data-ttu-id="f138f-1504">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="f138f-1504">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f138f-1505">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="f138f-1505">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f138f-1506">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="f138f-1506">Usage and limits reporting</span></span>
  - <span data-ttu-id="f138f-1507">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="f138f-1507">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f138f-1508">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="f138f-1508">Support for custom images</span></span>
  - <span data-ttu-id="f138f-1509">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1509">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f138f-1510">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="f138f-1510">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f138f-1511">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1511">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f138f-1512">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="f138f-1512">National clouds are supported</span></span>
* <span data-ttu-id="f138f-1513">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1513">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f138f-1514">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="f138f-1514">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f138f-1515">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1515">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f138f-1516">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="f138f-1516">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f138f-1517">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="f138f-1517">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f138f-1518">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="f138f-1518">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f138f-1519">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="f138f-1519">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f138f-1520">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1520">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f138f-1521">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="f138f-1521">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f138f-1522">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1522">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f138f-1523">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="f138f-1523">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f138f-1524">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1524">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f138f-1525">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="f138f-1525">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f138f-1526">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="f138f-1526">Billing</span></span>

* <span data-ttu-id="f138f-1527">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1527">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-1528">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-1528">Consumption</span></span>

* <span data-ttu-id="f138f-1529">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1529">Added `marketplace` commands</span></span>
* <span data-ttu-id="f138f-1530">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1530">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f138f-1531">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1531">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f138f-1532">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1532">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f138f-1533">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1533">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f138f-1534">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1534">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1535">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1535">Container</span></span>

* <span data-ttu-id="f138f-1536">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1536">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f138f-1537">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-1537">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1538">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1538">Extension</span></span>

* <span data-ttu-id="f138f-1539">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1539">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1540">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1540">Interactive</span></span>

* <span data-ttu-id="f138f-1541">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="f138f-1541">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f138f-1542">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1542">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f138f-1543">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1543">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1544">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1544">Network</span></span>

* <span data-ttu-id="f138f-1545">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-1545">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f138f-1546">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1546">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f138f-1547">#4910</span><span class="sxs-lookup"><span data-stu-id="f138f-1547">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f138f-1548">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1548">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f138f-1549">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1549">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f138f-1550">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1550">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f138f-1551">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1551">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f138f-1552">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1552">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-1553">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1553">Profile</span></span>

* <span data-ttu-id="f138f-1554">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1554">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f138f-1555">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1555">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-1556">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1556">RDBMS</span></span>

* <span data-ttu-id="f138f-1557">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1557">Added `georestore` command</span></span>
* <span data-ttu-id="f138f-1558">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1558">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1559">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1559">Resource</span></span>

* <span data-ttu-id="f138f-1560">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1560">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f138f-1561">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1561">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1562">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1562">SQL</span></span>

* <span data-ttu-id="f138f-1563">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1563">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1564">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1564">Storage</span></span>

* <span data-ttu-id="f138f-1565">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1565">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1566">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1566">VM</span></span>

* <span data-ttu-id="f138f-1567">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1567">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f138f-1568">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1568">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="f138f-1570">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1570">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f138f-1571">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="f138f-1571">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f138f-1572">#5718</span><span class="sxs-lookup"><span data-stu-id="f138f-1572">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f138f-1573">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="f138f-1573">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f138f-1574">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1574">March 27, 2018</span></span>

<span data-ttu-id="f138f-1575">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f138f-1575">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1576">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1576">Core</span></span>

* <span data-ttu-id="f138f-1577">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="f138f-1577">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1578">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1578">ACS</span></span>

* <span data-ttu-id="f138f-1579">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f138f-1579">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1580">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1580">Appservice</span></span>

* <span data-ttu-id="f138f-1581">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1581">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f138f-1582">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1582">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f138f-1583">Backup</span><span class="sxs-lookup"><span data-stu-id="f138f-1583">Backup</span></span>

* <span data-ttu-id="f138f-1584">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1584">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f138f-1585">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="f138f-1585">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f138f-1586">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="f138f-1586">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="f138f-1587">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="f138f-1587">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1588">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1588">Container</span></span>

* <span data-ttu-id="f138f-1589">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1589">Added `container exec` command.</span></span> <span data-ttu-id="f138f-1590">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f138f-1590">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f138f-1591">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f138f-1591">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1592">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1592">Extension</span></span>

* <span data-ttu-id="f138f-1593">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="f138f-1593">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f138f-1594">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-1594">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f138f-1595">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-1595">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1596">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1596">Interactive</span></span>

* <span data-ttu-id="f138f-1597">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-1597">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f138f-1598">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1598">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f138f-1599">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f138f-1599">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f138f-1600">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="f138f-1600">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f138f-1601">Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-1601">Lab</span></span>

* <span data-ttu-id="f138f-1602">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1602">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1603">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1603">Monitor</span></span>

* <span data-ttu-id="f138f-1604">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="f138f-1604">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f138f-1605">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="f138f-1605">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f138f-1606">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="f138f-1606">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1607">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1607">Network</span></span>

* <span data-ttu-id="f138f-1608">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1608">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-1609">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1609">Profile</span></span>

* <span data-ttu-id="f138f-1610">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1610">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-1611">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1611">RDBMS</span></span>

* <span data-ttu-id="f138f-1612">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1612">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1613">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1613">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f138f-1615">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1615">Role</span></span>

* <span data-ttu-id="f138f-1616">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1616">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f138f-1617">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f138f-1617">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f138f-1618">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1618">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f138f-1619">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1619">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f138f-1620">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1620">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1621">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1621">Storage</span></span>

* <span data-ttu-id="f138f-1622">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1622">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f138f-1623">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="f138f-1623">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1624">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1624">VM</span></span>

* <span data-ttu-id="f138f-1625">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1625">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f138f-1626">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1626">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f138f-1627">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="f138f-1627">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f138f-1628">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f138f-1628">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f138f-1629">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1629">March 13, 2018</span></span>

<span data-ttu-id="f138f-1630">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f138f-1630">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1631">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1631">ACR</span></span>

* <span data-ttu-id="f138f-1632">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1632">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f138f-1633">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1633">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f138f-1634">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1634">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1635">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1635">ACS</span></span>

* <span data-ttu-id="f138f-1636">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1636">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f138f-1637">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1637">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f138f-1638">Advisor</span><span class="sxs-lookup"><span data-stu-id="f138f-1638">Advisor</span></span>

* <span data-ttu-id="f138f-1639">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1639">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f138f-1640">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1640">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f138f-1641">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1641">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f138f-1642">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1642">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f138f-1643">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1643">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1644">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1644">Appservice</span></span>

* <span data-ttu-id="f138f-1645">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1645">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f138f-1646">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1646">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f138f-1647">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f138f-1647">Eventhubs</span></span>

* <span data-ttu-id="f138f-1648">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1648">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1649">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1649">Extension</span></span>

* <span data-ttu-id="f138f-1650">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="f138f-1650">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1651">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1651">Interactive</span></span>

* <span data-ttu-id="f138f-1652">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="f138f-1652">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f138f-1653">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="f138f-1653">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f138f-1654">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1654">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f138f-1655">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1655">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1656">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1656">Monitor</span></span>

* <span data-ttu-id="f138f-1657">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1657">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f138f-1658">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1658">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f138f-1659">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1659">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f138f-1660">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1660">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1661">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1661">Network</span></span>

* <span data-ttu-id="f138f-1662">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1662">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f138f-1663">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="f138f-1663">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f138f-1664">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1664">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f138f-1665">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1665">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-1666">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1666">Profile</span></span>

* <span data-ttu-id="f138f-1667">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1667">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f138f-1668">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1668">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-1669">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-1669">RDBMS</span></span>

* <span data-ttu-id="f138f-1670">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1670">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f138f-1671">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f138f-1671">Service Bus</span></span>

* <span data-ttu-id="f138f-1672">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1672">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1673">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1673">Storage</span></span>

* <span data-ttu-id="f138f-1674">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="f138f-1674">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f138f-1675">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="f138f-1675">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1676">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1676">VM</span></span>

* <span data-ttu-id="f138f-1677">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="f138f-1677">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f138f-1678">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1678">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f138f-1679">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1679">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f138f-1680">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1680">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f138f-1681">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1681">February 27, 2018</span></span>

<span data-ttu-id="f138f-1682">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f138f-1682">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1683">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1683">Core</span></span>

* <span data-ttu-id="f138f-1684">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="f138f-1684">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f138f-1685">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1685">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f138f-1686">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1686">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1687">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1687">ACS</span></span>

* <span data-ttu-id="f138f-1688">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1688">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f138f-1689">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f138f-1689">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f138f-1690">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1690">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f138f-1691">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1691">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1692">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1692">Appservice</span></span>

* <span data-ttu-id="f138f-1693">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f138f-1693">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f138f-1694">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="f138f-1694">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f138f-1695">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f138f-1695">Cognitive Services</span></span>

* <span data-ttu-id="f138f-1696">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1696">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-1697">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-1697">Consumption</span></span>

* <span data-ttu-id="f138f-1698">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1698">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f138f-1699">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1699">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1700">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1700">Container</span></span>

* <span data-ttu-id="f138f-1701">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="f138f-1701">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1702">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1702">Network</span></span>

* <span data-ttu-id="f138f-1703">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f138f-1703">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1704">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1704">Resource</span></span>

* <span data-ttu-id="f138f-1705">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="f138f-1705">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1706">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1706">Role</span></span>

* <span data-ttu-id="f138f-1707">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1707">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1708">SQL</span></span>

* <span data-ttu-id="f138f-1709">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="f138f-1709">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1710">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1710">Storage</span></span>

* <span data-ttu-id="f138f-1711">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-1711">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1712">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1712">VM</span></span>

* <span data-ttu-id="f138f-1713">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1713">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f138f-1714">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1714">February 13, 2018</span></span>

<span data-ttu-id="f138f-1715">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f138f-1715">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1716">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1716">Core</span></span>

* <span data-ttu-id="f138f-1717">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1717">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1718">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1718">ACS</span></span>

* <span data-ttu-id="f138f-1719">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1719">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f138f-1720">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1720">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f138f-1721">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1721">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f138f-1722">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1722">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f138f-1723">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1723">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f138f-1724">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1724">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f138f-1725">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f138f-1725">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f138f-1726">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="f138f-1726">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1727">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1727">Appservice</span></span>

* <span data-ttu-id="f138f-1728">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="f138f-1728">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f138f-1729">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1729">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-1730">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-1730">CDN</span></span>

* <span data-ttu-id="f138f-1731">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1731">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1732">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1732">Container</span></span>

* <span data-ttu-id="f138f-1733">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1733">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f138f-1734">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1734">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-1735">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-1735">CosmosDB</span></span>

* <span data-ttu-id="f138f-1736">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1736">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1737">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1737">Extension</span></span>

* <span data-ttu-id="f138f-1738">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1738">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f138f-1739">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1739">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f138f-1740">Feedback</span><span class="sxs-lookup"><span data-stu-id="f138f-1740">Feedback</span></span>

* <span data-ttu-id="f138f-1741">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1741">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1742">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1742">Interactive</span></span>

* <span data-ttu-id="f138f-1743">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1743">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f138f-1744">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1744">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-1745">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1745">IoT</span></span>

* <span data-ttu-id="f138f-1746">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f138f-1746">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f138f-1747">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f138f-1747">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f138f-1748">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1748">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f138f-1749">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1749">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1750">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1750">Monitor</span></span>

* <span data-ttu-id="f138f-1751">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1751">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1752">Network</span></span>

* <span data-ttu-id="f138f-1753">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="f138f-1753">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f138f-1754">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1754">Profile</span></span>

* <span data-ttu-id="f138f-1755">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="f138f-1755">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1756">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1756">Resource</span></span>

* <span data-ttu-id="f138f-1757">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1757">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1758">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1758">Role</span></span>

* <span data-ttu-id="f138f-1759">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1759">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1760">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1760">SQL</span></span>

* <span data-ttu-id="f138f-1761">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1761">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f138f-1762">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1762">Added `sql db rename`</span></span>
* <span data-ttu-id="f138f-1763">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1763">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1764">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1764">Storage</span></span>

* <span data-ttu-id="f138f-1765">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1765">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1766">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1766">VM</span></span>

* <span data-ttu-id="f138f-1767">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1767">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f138f-1768">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1768">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f138f-1769">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f138f-1769">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f138f-1770">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1770">January 31, 2018</span></span>

<span data-ttu-id="f138f-1771">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f138f-1771">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1772">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1772">Core</span></span>

* <span data-ttu-id="f138f-1773">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1773">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f138f-1774">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1774">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f138f-1775">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f138f-1775">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f138f-1776">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f138f-1776">Use `--verbose` to see</span></span>
* <span data-ttu-id="f138f-1777">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1777">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1778">ACS</span></span>

* <span data-ttu-id="f138f-1779">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="f138f-1779">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f138f-1780">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1780">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1781">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1781">Appservice</span></span>

* <span data-ttu-id="f138f-1782">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f138f-1782">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f138f-1783">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1783">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-1784">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-1784">CDN</span></span>

* <span data-ttu-id="f138f-1785">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1785">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-1786">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-1786">CosmosDB</span></span>

* <span data-ttu-id="f138f-1787">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1787">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1788">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1788">Interactive</span></span>

* <span data-ttu-id="f138f-1789">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1789">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1790">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1790">Network</span></span>

* <span data-ttu-id="f138f-1791">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1791">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f138f-1792">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="f138f-1792">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f138f-1793">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1793">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f138f-1794">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1794">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f138f-1795">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1795">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f138f-1796">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="f138f-1796">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f138f-1797">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1797">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f138f-1798">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1798">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f138f-1799">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1799">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f138f-1800">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="f138f-1800">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-1801">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1801">Profile</span></span>

* <span data-ttu-id="f138f-1802">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1802">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1803">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1803">Resource</span></span>

* <span data-ttu-id="f138f-1804">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="f138f-1804">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1805">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1805">Storage</span></span>

* <span data-ttu-id="f138f-1806">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1806">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f138f-1807">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1807">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f138f-1808">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f138f-1808">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f138f-1809">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1809">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f138f-1810">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="f138f-1810">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1811">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1811">VM</span></span>

* <span data-ttu-id="f138f-1812">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1812">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f138f-1813">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="f138f-1813">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f138f-1814">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1814">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f138f-1815">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1815">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f138f-1816">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f138f-1816">January 17, 2018</span></span>

<span data-ttu-id="f138f-1817">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f138f-1817">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1818">ACR</span></span>

* <span data-ttu-id="f138f-1819">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1819">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f138f-1820">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="f138f-1820">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1821">ACS</span></span>

* <span data-ttu-id="f138f-1822">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1822">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f138f-1823">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1823">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1824">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1824">Appservice</span></span>

* <span data-ttu-id="f138f-1825">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="f138f-1825">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f138f-1826">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1826">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f138f-1827">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1827">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f138f-1828">Backup</span><span class="sxs-lookup"><span data-stu-id="f138f-1828">Backup</span></span>

* <span data-ttu-id="f138f-1829">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="f138f-1829">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f138f-1830">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1830">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f138f-1831">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="f138f-1831">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f138f-1832">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-1832">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f138f-1833">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="f138f-1833">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1834">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1834">Batch</span></span>

* <span data-ttu-id="f138f-1835">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f138f-1835">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f138f-1836">Cloud</span><span class="sxs-lookup"><span data-stu-id="f138f-1836">Cloud</span></span>

* <span data-ttu-id="f138f-1837">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1837">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-1838">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-1838">Consumption</span></span>

* <span data-ttu-id="f138f-1839">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f138f-1839">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f138f-1840">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f138f-1840">Event Grid</span></span>

* <span data-ttu-id="f138f-1841">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-1841">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f138f-1842">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-1842">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f138f-1843">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1843">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f138f-1844">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1844">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f138f-1845">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1845">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f138f-1846">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1846">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f138f-1847">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1847">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f138f-1848">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1848">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-1849">Interactive</span><span class="sxs-lookup"><span data-stu-id="f138f-1849">Interactive</span></span>

* <span data-ttu-id="f138f-1850">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-1850">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f138f-1851">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1851">Fixed errors on startup</span></span>
* <span data-ttu-id="f138f-1852">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-1852">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-1853">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1853">IoT</span></span>

* <span data-ttu-id="f138f-1854">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1854">Added support for device provisioning service</span></span>
* <span data-ttu-id="f138f-1855">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1855">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f138f-1856">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="f138f-1856">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1857">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1857">Monitor</span></span>

* <span data-ttu-id="f138f-1858">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1858">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f138f-1859">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f138f-1859">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f138f-1860">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1860">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1861">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1861">Network</span></span>

* <span data-ttu-id="f138f-1862">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-1862">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f138f-1863">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1863">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-1864">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-1864">Profile</span></span>

* <span data-ttu-id="f138f-1865">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1865">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1866">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1866">Role</span></span>

* <span data-ttu-id="f138f-1867">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="f138f-1867">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f138f-1868">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f138f-1868">Service Fabric</span></span>

* <span data-ttu-id="f138f-1869">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1869">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f138f-1870">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1870">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1871">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1871">VM</span></span>

* <span data-ttu-id="f138f-1872">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="f138f-1872">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f138f-1873">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1873">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f138f-1874">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="f138f-1874">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f138f-1875">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1875">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f138f-1876">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1876">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f138f-1877">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1877">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f138f-1878">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1878">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f138f-1879">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1879">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f138f-1880">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-1880">December 19, 2017</span></span>

<span data-ttu-id="f138f-1881">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f138f-1881">Version 2.0.23</span></span>

* <span data-ttu-id="f138f-1882">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1882">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1883">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1883">Container</span></span>

* <span data-ttu-id="f138f-1884">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1884">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1885">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1885">Network</span></span>

* <span data-ttu-id="f138f-1886">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1886">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f138f-1887">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1887">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1888">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1888">Storage</span></span>

* <span data-ttu-id="f138f-1889">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1889">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1890">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1890">VM</span></span>

* <span data-ttu-id="f138f-1891">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1891">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f138f-1892">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-1892">December 5, 2017</span></span>

<span data-ttu-id="f138f-1893">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f138f-1893">Version 2.0.22</span></span>

* <span data-ttu-id="f138f-1894">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1894">Removed `az component` commands.</span></span> <span data-ttu-id="f138f-1895">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1895">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1896">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1896">Core</span></span>
* <span data-ttu-id="f138f-1897">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1897">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f138f-1898">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1898">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1899">ACS</span></span>

* <span data-ttu-id="f138f-1900">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1900">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f138f-1901">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="f138f-1901">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f138f-1902">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="f138f-1902">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f138f-1903">Advisor</span><span class="sxs-lookup"><span data-stu-id="f138f-1903">Advisor</span></span>

* <span data-ttu-id="f138f-1904">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-1904">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1905">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1905">Appservice</span></span>

* <span data-ttu-id="f138f-1906">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f138f-1906">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f138f-1907">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f138f-1907">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f138f-1908">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1908">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f138f-1909">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f138f-1909">Consumption</span></span>

* <span data-ttu-id="f138f-1910">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1910">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1911">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1911">Container</span></span>

* <span data-ttu-id="f138f-1912">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="f138f-1912">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1913">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1913">Monitor</span></span>

* <span data-ttu-id="f138f-1914">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1914">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1915">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1915">Resource</span></span>

* <span data-ttu-id="f138f-1916">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1916">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f138f-1917">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-1917">Role</span></span>

* <span data-ttu-id="f138f-1918">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1918">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f138f-1919">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1919">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f138f-1920">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f138f-1920">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1921">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1921">SQL</span></span>

* <span data-ttu-id="f138f-1922">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1922">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f138f-1923">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-1923">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1924">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1924">VM</span></span>

* <span data-ttu-id="f138f-1925">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1925">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f138f-1926">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-1926">November 14, 2017</span></span>

<span data-ttu-id="f138f-1927">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f138f-1927">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1928">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1928">ACR</span></span>

* <span data-ttu-id="f138f-1929">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1929">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f138f-1930">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-1930">ACS</span></span>

* <span data-ttu-id="f138f-1931">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1931">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f138f-1932">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f138f-1932">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f138f-1933">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="f138f-1933">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f138f-1934">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1934">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f138f-1935">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1935">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-1936">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-1936">Appservice</span></span>

* <span data-ttu-id="f138f-1937">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1937">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f138f-1938">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1938">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f138f-1939">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-1939">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f138f-1940">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-1940">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f138f-1941">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1941">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f138f-1942">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f138f-1942">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-1943">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-1943">Batch</span></span>

* <span data-ttu-id="f138f-1944">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f138f-1944">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-1945">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f138f-1945">Batchai</span></span>

* <span data-ttu-id="f138f-1946">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1946">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f138f-1947">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1947">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f138f-1948">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1948">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f138f-1949">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1949">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f138f-1950">Cloud</span><span class="sxs-lookup"><span data-stu-id="f138f-1950">Cloud</span></span>

* <span data-ttu-id="f138f-1951">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="f138f-1951">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f138f-1952">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-1952">Container</span></span>

* <span data-ttu-id="f138f-1953">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1953">Added support to open multiple ports</span></span>
* <span data-ttu-id="f138f-1954">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1954">Added container group restart policy</span></span>
* <span data-ttu-id="f138f-1955">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1955">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f138f-1956">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-1956">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f138f-1957">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f138f-1957">Data Lake Analytics</span></span>

* <span data-ttu-id="f138f-1958">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f138f-1958">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f138f-1959">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f138f-1959">Data Lake Store</span></span>

* <span data-ttu-id="f138f-1960">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f138f-1960">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-1961">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-1961">Extension</span></span>

* <span data-ttu-id="f138f-1962">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1962">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f138f-1963">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f138f-1963">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-1964">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-1964">IoT</span></span>

* <span data-ttu-id="f138f-1965">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1965">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-1966">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-1966">Monitor</span></span>

* <span data-ttu-id="f138f-1967">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1967">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f138f-1968">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-1968">Network</span></span>

* <span data-ttu-id="f138f-1969">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1969">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f138f-1970">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-1970">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f138f-1971">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f138f-1971">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f138f-1972">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1972">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f138f-1973">Reservations</span><span class="sxs-lookup"><span data-stu-id="f138f-1973">Reservations</span></span>

* <span data-ttu-id="f138f-1974">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f138f-1974">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-1975">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-1975">Resource</span></span>

* <span data-ttu-id="f138f-1976">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1976">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-1977">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-1977">SQL</span></span>

* <span data-ttu-id="f138f-1978">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1978">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-1979">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-1979">Storage</span></span>

* <span data-ttu-id="f138f-1980">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f138f-1980">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f138f-1981">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="f138f-1981">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f138f-1982">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f138f-1982">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f138f-1983">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1983">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f138f-1984">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1984">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f138f-1985">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-1985">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f138f-1986">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-1986">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-1987">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-1987">VM</span></span>

* <span data-ttu-id="f138f-1988">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f138f-1988">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f138f-1989">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1989">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f138f-1990">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="f138f-1990">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f138f-1991">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-1991">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f138f-1992">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-1992">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f138f-1993">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-1993">October 24, 2017</span></span>

<span data-ttu-id="f138f-1994">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f138f-1994">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f138f-1995">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-1995">Core</span></span>

* <span data-ttu-id="f138f-1996">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="f138f-1996">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-1997">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-1997">ACR</span></span>

* <span data-ttu-id="f138f-1998">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="f138f-1998">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f138f-1999">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f138f-1999">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f138f-2000">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2000">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2001">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2001">ACS</span></span>

* <span data-ttu-id="f138f-2002">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2002">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f138f-2003">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2003">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2004">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2004">Appservice</span></span>

* <span data-ttu-id="f138f-2005">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="f138f-2005">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f138f-2006">Komponente</span><span class="sxs-lookup"><span data-stu-id="f138f-2006">Component</span></span>

* <span data-ttu-id="f138f-2007">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2007">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-2008">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-2008">Monitor</span></span>

* <span data-ttu-id="f138f-2009">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2009">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2010">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2010">Resource</span></span>

* <span data-ttu-id="f138f-2011">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2011">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f138f-2012">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="f138f-2012">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2013">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2013">VM</span></span>

* <span data-ttu-id="f138f-2014">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2014">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f138f-2015">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2015">October 9, 2017</span></span>

<span data-ttu-id="f138f-2016">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f138f-2016">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f138f-2017">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-2017">Core</span></span>

* <span data-ttu-id="f138f-2018">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2018">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2019">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2019">Appservice</span></span>

* <span data-ttu-id="f138f-2020">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2020">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-2021">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-2021">Batch</span></span>

* <span data-ttu-id="f138f-2022">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f138f-2022">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f138f-2023">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2023">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f138f-2024">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2024">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f138f-2025">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2025">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f138f-2026">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f138f-2026">Batchai</span></span>

* <span data-ttu-id="f138f-2027">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2027">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-2028">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-2028">Keyvault</span></span>

* <span data-ttu-id="f138f-2029">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="f138f-2029">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f138f-2030">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f138f-2030">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f138f-2031">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2031">Network</span></span>

* <span data-ttu-id="f138f-2032">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f138f-2032">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f138f-2033">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2033">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2034">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2034">Resource</span></span>

* <span data-ttu-id="f138f-2035">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2035">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f138f-2036">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2036">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f138f-2037">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2037">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f138f-2038">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2038">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-2039">Sql</span><span class="sxs-lookup"><span data-stu-id="f138f-2039">Sql</span></span>

* <span data-ttu-id="f138f-2040">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2040">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f138f-2041">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2041">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f138f-2042">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2042">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2043">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2043">Storage</span></span>

* <span data-ttu-id="f138f-2044">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2044">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2045">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2045">Vm</span></span>

* <span data-ttu-id="f138f-2046">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="f138f-2046">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f138f-2047">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2047">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f138f-2048">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2048">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f138f-2049">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2049">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f138f-2050">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2050">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f138f-2051">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2051">September 22, 2017</span></span>

<span data-ttu-id="f138f-2052">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f138f-2052">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2053">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2053">Resource</span></span>

* <span data-ttu-id="f138f-2054">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2054">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f138f-2055">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2055">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f138f-2056">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2056">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f138f-2057">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="f138f-2057">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2058">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2058">Network</span></span>

* <span data-ttu-id="f138f-2059">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2059">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f138f-2060">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2060">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f138f-2061">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2061">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f138f-2062">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2062">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f138f-2063">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2063">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f138f-2064">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2064">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f138f-2065">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2065">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2066">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2066">Storage</span></span>

* <span data-ttu-id="f138f-2067">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f138f-2067">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f138f-2068">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="f138f-2068">Eventgrid</span></span>

* <span data-ttu-id="f138f-2069">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2069">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-2070">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-2070">SQL</span></span>

* <span data-ttu-id="f138f-2071">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="f138f-2071">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f138f-2072">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f138f-2072">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f138f-2073">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2073">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-2074">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-2074">Keyvault</span></span>

* <span data-ttu-id="f138f-2075">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2075">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2076">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2076">VM</span></span>

* <span data-ttu-id="f138f-2077">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2077">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f138f-2078">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f138f-2078">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f138f-2079">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2079">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f138f-2080">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2080">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f138f-2081">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2081">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f138f-2082">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2082">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2083">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2083">ACS</span></span>

* <span data-ttu-id="f138f-2084">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2084">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2085">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2085">Appservice</span></span>

* <span data-ttu-id="f138f-2086">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f138f-2086">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f138f-2087">Backup</span><span class="sxs-lookup"><span data-stu-id="f138f-2087">Backup</span></span>

* <span data-ttu-id="f138f-2088">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f138f-2088">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f138f-2089">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2089">September 11, 2017</span></span>

<span data-ttu-id="f138f-2090">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f138f-2090">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f138f-2091">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-2091">Core</span></span>

* <span data-ttu-id="f138f-2092">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="f138f-2092">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f138f-2093">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="f138f-2093">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2094">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2094">Acs</span></span>

* <span data-ttu-id="f138f-2095">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2095">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f138f-2096">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2096">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2097">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2097">Appservice</span></span>

* <span data-ttu-id="f138f-2098">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="f138f-2098">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-2099">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-2099">CDN</span></span>

* <span data-ttu-id="f138f-2100">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f138f-2100">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f138f-2101">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f138f-2101">Extension</span></span>

* <span data-ttu-id="f138f-2102">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-2102">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-2103">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-2103">Keyvault</span></span>

* <span data-ttu-id="f138f-2104">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="f138f-2104">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2105">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2105">Network</span></span>

* <span data-ttu-id="f138f-2106">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2106">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f138f-2107">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2107">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f138f-2108">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2108">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f138f-2109">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2109">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f138f-2110">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2110">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2111">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2111">Resource</span></span>

* <span data-ttu-id="f138f-2112">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="f138f-2112">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f138f-2113">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="f138f-2113">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f138f-2114">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="f138f-2114">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f138f-2115">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="f138f-2115">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-2116">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-2116">SQL</span></span>

* <span data-ttu-id="f138f-2117">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2117">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2118">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2118">VM</span></span>

* <span data-ttu-id="f138f-2119">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f138f-2119">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f138f-2120">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="f138f-2120">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f138f-2121">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2121">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f138f-2122">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="f138f-2122">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f138f-2123">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="f138f-2123">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f138f-2124">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2124">August 31, 2017</span></span>

<span data-ttu-id="f138f-2125">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f138f-2125">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-2126">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-2126">Keyvault</span></span>

* <span data-ttu-id="f138f-2127">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="f138f-2127">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f138f-2128">Sf</span><span class="sxs-lookup"><span data-stu-id="f138f-2128">Sf</span></span>

* <span data-ttu-id="f138f-2129">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2129">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2130">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2130">Storage</span></span>

* <span data-ttu-id="f138f-2131">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="f138f-2131">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f138f-2132">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="f138f-2132">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f138f-2133">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2133">August 28, 2017</span></span>

<span data-ttu-id="f138f-2134">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f138f-2134">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f138f-2135">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f138f-2135">CLI</span></span>

* <span data-ttu-id="f138f-2136">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2136">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2137">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2137">ACS</span></span>

* <span data-ttu-id="f138f-2138">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2138">Corrected preview regions</span></span>
* <span data-ttu-id="f138f-2139">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2139">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f138f-2140">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2140">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2141">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2141">Appservice</span></span>

* <span data-ttu-id="f138f-2142">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2142">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f138f-2143">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2143">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f138f-2144">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2144">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f138f-2145">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="f138f-2145">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f138f-2146">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2146">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-2147">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-2147">IoT</span></span>

* <span data-ttu-id="f138f-2148">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f138f-2148">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2149">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2149">Network</span></span>

* <span data-ttu-id="f138f-2150">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2150">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f138f-2151">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2151">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f138f-2152">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2152">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f138f-2153">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2153">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f138f-2154">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2154">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-2155">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-2155">Profile</span></span>

* <span data-ttu-id="f138f-2156">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2156">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f138f-2157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f138f-2157">Service Fabric</span></span>

* <span data-ttu-id="f138f-2158">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f138f-2158">Preview release</span></span>
* <span data-ttu-id="f138f-2159">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2159">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f138f-2160">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2160">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f138f-2161">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2161">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2162">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2162">Storage</span></span>

* <span data-ttu-id="f138f-2163">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2163">Enabled setting blob tier</span></span>
* <span data-ttu-id="f138f-2164">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2164">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f138f-2165">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2165">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f138f-2166">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2166">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f138f-2167">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2167">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f138f-2168">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="f138f-2168">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2169">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2169">VM</span></span>

* <span data-ttu-id="f138f-2170">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-2170">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f138f-2171">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-2171">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f138f-2172">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2172">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f138f-2173">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-2173">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f138f-2174">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2174">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f138f-2175">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-2175">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f138f-2176">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2176">August 15, 2017</span></span>

<span data-ttu-id="f138f-2177">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f138f-2177">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2178">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2178">ACS</span></span>

* <span data-ttu-id="f138f-2179">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2179">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2180">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2180">Appservice</span></span>

* <span data-ttu-id="f138f-2181">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2181">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f138f-2182">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f138f-2182">Event Grid</span></span>

* <span data-ttu-id="f138f-2183">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2183">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f138f-2184">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2184">August 11, 2017</span></span>

<span data-ttu-id="f138f-2185">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f138f-2185">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2186">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2186">ACS</span></span>

* <span data-ttu-id="f138f-2187">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2187">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-2188">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-2188">Batch</span></span>

* <span data-ttu-id="f138f-2189">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2189">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f138f-2190">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2190">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f138f-2191">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2191">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f138f-2192">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="f138f-2192">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f138f-2193">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="f138f-2193">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f138f-2194">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2194">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f138f-2195">Komponente</span><span class="sxs-lookup"><span data-stu-id="f138f-2195">Component</span></span>

* <span data-ttu-id="f138f-2196">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2196">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f138f-2197">Container</span><span class="sxs-lookup"><span data-stu-id="f138f-2197">Container</span></span>

* <span data-ttu-id="f138f-2198">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="f138f-2198">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f138f-2199">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f138f-2199">Data Lake Store</span></span>

* <span data-ttu-id="f138f-2200">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2200">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f138f-2201">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f138f-2201">Event Grid</span></span>

* <span data-ttu-id="f138f-2202">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f138f-2202">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2203">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2203">Network</span></span>

* <span data-ttu-id="f138f-2204">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-2204">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f138f-2205">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-2205">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f138f-2206">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-2206">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f138f-2207">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f138f-2207">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-2208">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-2208">Profile</span></span>

* <span data-ttu-id="f138f-2209">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="f138f-2209">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2210">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2210">Storage</span></span>

* <span data-ttu-id="f138f-2211">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2211">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2212">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2212">VM</span></span>

* <span data-ttu-id="f138f-2213">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2213">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f138f-2214">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2214">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f138f-2215">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2215">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f138f-2216">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="f138f-2216">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f138f-2217">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2217">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f138f-2218">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2218">July 28, 2017</span></span>

<span data-ttu-id="f138f-2219">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f138f-2219">Version 2.0.12</span></span>

* <span data-ttu-id="f138f-2220">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2220">Added container commands</span></span>
* <span data-ttu-id="f138f-2221">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2221">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="f138f-2222">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-2222">Core</span></span>

* <span data-ttu-id="f138f-2223">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="f138f-2223">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f138f-2224">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2224">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f138f-2225">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="f138f-2225">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f138f-2226">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="f138f-2226">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f138f-2227">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="f138f-2227">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f138f-2228">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="f138f-2228">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f138f-2229">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f138f-2229">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f138f-2230">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="f138f-2230">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f138f-2231">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="f138f-2231">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f138f-2232">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-2232">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f138f-2233">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="f138f-2233">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f138f-2234">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="f138f-2234">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f138f-2235">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f138f-2235">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f138f-2236">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f138f-2236">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f138f-2237">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f138f-2237">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f138f-2238">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="f138f-2238">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f138f-2239">ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-2239">ACR</span></span>

* <span data-ttu-id="f138f-2240">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2240">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f138f-2241">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2241">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f138f-2242">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2242">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f138f-2243">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2243">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f138f-2244">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2244">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f138f-2245">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2245">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2246">ACS</span></span>

* <span data-ttu-id="f138f-2247">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f138f-2247">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2248">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2248">Appservice</span></span>

* <span data-ttu-id="f138f-2249">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="f138f-2249">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f138f-2250">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="f138f-2250">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f138f-2251">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f138f-2251">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f138f-2252">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="f138f-2252">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f138f-2253">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="f138f-2253">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f138f-2254">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="f138f-2254">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f138f-2255">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="f138f-2255">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f138f-2256">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="f138f-2256">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f138f-2257">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2257">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f138f-2258">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="f138f-2258">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f138f-2259">Batch</span><span class="sxs-lookup"><span data-stu-id="f138f-2259">Batch</span></span>

* <span data-ttu-id="f138f-2260">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2260">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f138f-2261">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2261">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f138f-2262">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2262">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f138f-2263">CDN</span><span class="sxs-lookup"><span data-stu-id="f138f-2263">CDN</span></span>

* <span data-ttu-id="f138f-2264">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f138f-2264">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f138f-2265">Cloud</span><span class="sxs-lookup"><span data-stu-id="f138f-2265">Cloud</span></span>

* <span data-ttu-id="f138f-2266">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="f138f-2266">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f138f-2267">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="f138f-2267">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f138f-2268">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f138f-2268">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f138f-2269">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="f138f-2269">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f138f-2270">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f138f-2270">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-2271">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-2271">CosmosDB</span></span>

* <span data-ttu-id="f138f-2272">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="f138f-2272">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f138f-2273">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2273">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f138f-2274">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f138f-2274">Data Lake Analytics</span></span>

* <span data-ttu-id="f138f-2275">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2275">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f138f-2276">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2276">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f138f-2277">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2277">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f138f-2278">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f138f-2278">Data Lake Store</span></span>

* <span data-ttu-id="f138f-2279">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2279">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f138f-2280">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f138f-2280">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f138f-2281">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2281">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f138f-2282">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f138f-2282">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f138f-2283">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="f138f-2283">Interactive</span></span>

* <span data-ttu-id="f138f-2284">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-2284">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f138f-2285">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-2285">Increased test coverage</span></span>
* <span data-ttu-id="f138f-2286">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-2286">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f138f-2287">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="f138f-2287">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f138f-2288">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="f138f-2288">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f138f-2289">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="f138f-2289">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f138f-2290">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f138f-2290">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f138f-2291">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2291">Added `--progress` flag</span></span>
* <span data-ttu-id="f138f-2292">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2292">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f138f-2293">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="f138f-2293">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f138f-2294">IoT</span><span class="sxs-lookup"><span data-stu-id="f138f-2294">IoT</span></span>

* <span data-ttu-id="f138f-2295">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f138f-2295">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f138f-2296">(3934)</span><span class="sxs-lookup"><span data-stu-id="f138f-2296">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f138f-2297">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="f138f-2297">Key vault</span></span>

* <span data-ttu-id="f138f-2298">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f138f-2298">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f138f-2299">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f138f-2299">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f138f-2300">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f138f-2300">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f138f-2301">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f138f-2301">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f138f-2302">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f138f-2302">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f138f-2303">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="f138f-2303">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f138f-2304">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2304">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f138f-2305">(3307)</span><span class="sxs-lookup"><span data-stu-id="f138f-2305">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f138f-2306">Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-2306">Lab</span></span>

* <span data-ttu-id="f138f-2307">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2307">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f138f-2308">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2308">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-2309">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-2309">Monitor</span></span>

* <span data-ttu-id="f138f-2310">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="f138f-2310">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f138f-2311">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2311">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f138f-2312">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2312">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f138f-2313">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2313">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f138f-2314">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f138f-2314">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f138f-2315">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="f138f-2315">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f138f-2316">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="f138f-2316">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f138f-2317">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="f138f-2317">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f138f-2318">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="f138f-2318">`location` no longer required</span></span>
  * <span data-ttu-id="f138f-2319">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="f138f-2319">Add name and ID support for target</span></span>
  * <span data-ttu-id="f138f-2320">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f138f-2320">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f138f-2321">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="f138f-2321">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f138f-2322">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2322">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f138f-2323">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="f138f-2323">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f138f-2324">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f138f-2324">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f138f-2325">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2325">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2326">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2326">Network</span></span>

* <span data-ttu-id="f138f-2327">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2327">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f138f-2328">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2328">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f138f-2329">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f138f-2329">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f138f-2330">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f138f-2330">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f138f-2331">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f138f-2331">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f138f-2332">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2332">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f138f-2333">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f138f-2333">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f138f-2334">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f138f-2334">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f138f-2335">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f138f-2335">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f138f-2336">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f138f-2336">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f138f-2337">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2337">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f138f-2338">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2338">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f138f-2339">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f138f-2339">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f138f-2340">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2340">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f138f-2341">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2341">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f138f-2342">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2342">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f138f-2343">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="f138f-2343">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f138f-2344">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-2344">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f138f-2345">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2345">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f138f-2346">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2346">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f138f-2347">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f138f-2347">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f138f-2348">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f138f-2348">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f138f-2349">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-2349">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f138f-2350">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f138f-2350">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f138f-2351">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f138f-2351">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f138f-2352">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f138f-2352">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f138f-2353">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f138f-2353">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-2354">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-2354">Profile</span></span>

* <span data-ttu-id="f138f-2355">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="f138f-2355">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f138f-2356">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="f138f-2356">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f138f-2357">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="f138f-2357">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f138f-2358">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2358">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f138f-2359">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="f138f-2359">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f138f-2360">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f138f-2360">RDBMS</span></span>

* <span data-ttu-id="f138f-2361">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="f138f-2361">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f138f-2362">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="f138f-2362">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f138f-2363">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="f138f-2363">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f138f-2364">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="f138f-2364">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2365">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2365">Resource</span></span>

* <span data-ttu-id="f138f-2366">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-2366">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f138f-2367">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="f138f-2367">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f138f-2368">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-2368">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f138f-2369">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f138f-2369">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f138f-2370">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="f138f-2370">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f138f-2371">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="f138f-2371">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f138f-2372">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="f138f-2372">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f138f-2373">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2373">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f138f-2374">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-2374">Role</span></span>

* <span data-ttu-id="f138f-2375">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f138f-2375">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f138f-2376">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="f138f-2376">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f138f-2377">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="f138f-2377">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f138f-2378">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f138f-2378">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f138f-2379">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2379">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f138f-2380">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f138f-2380">Service Fabric</span></span>
* <span data-ttu-id="f138f-2381">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="f138f-2381">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f138f-2382">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="f138f-2382">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f138f-2383">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="f138f-2383">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-2384">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-2384">SQL</span></span>

* <span data-ttu-id="f138f-2385">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2385">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f138f-2386">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f138f-2386">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f138f-2387">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2387">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2388">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2388">Storage</span></span>

* <span data-ttu-id="f138f-2389">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="f138f-2389">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f138f-2390">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2390">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f138f-2391">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="f138f-2391">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f138f-2392">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="f138f-2392">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f138f-2393">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="f138f-2393">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f138f-2394">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="f138f-2394">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2395">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2395">VM</span></span>

* <span data-ttu-id="f138f-2396">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f138f-2396">Support configuring nsg</span></span>
* <span data-ttu-id="f138f-2397">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-2397">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f138f-2398">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="f138f-2398">Support managed service identities</span></span>
* <span data-ttu-id="f138f-2399">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="f138f-2399">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f138f-2400">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="f138f-2400">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f138f-2401">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2401">May 10, 2017</span></span>

<span data-ttu-id="f138f-2402">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f138f-2402">Version 2.0.6</span></span>

* <span data-ttu-id="f138f-2403">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="f138f-2403">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f138f-2404">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="f138f-2404">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f138f-2405">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="f138f-2405">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f138f-2406">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2406">Include Cognitive Services module</span></span>
* <span data-ttu-id="f138f-2407">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2407">Include Service Fabric module</span></span>
* <span data-ttu-id="f138f-2408">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="f138f-2408">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f138f-2409">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="f138f-2409">Add support for CDN commands</span></span>
* <span data-ttu-id="f138f-2410">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2410">Remove Container module</span></span>
* <span data-ttu-id="f138f-2411">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f138f-2411">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f138f-2412">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f138f-2412">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="f138f-2413">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-2413">Core</span></span>

* <span data-ttu-id="f138f-2414">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="f138f-2414">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f138f-2415">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f138f-2415">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f138f-2416">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f138f-2416">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f138f-2417">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f138f-2417">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f138f-2418">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f138f-2418">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f138f-2419">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f138f-2419">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f138f-2420">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f138f-2420">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f138f-2421">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f138f-2421">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f138f-2422">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f138f-2422">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f138f-2423">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="f138f-2423">core: Improved performance</span></span>
* <span data-ttu-id="f138f-2424">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="f138f-2424">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f138f-2425">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="f138f-2425">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2426">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2426">ACS</span></span>

* <span data-ttu-id="f138f-2427">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f138f-2427">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f138f-2428">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="f138f-2428">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f138f-2429">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2429">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f138f-2430">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f138f-2430">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2431">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2431">AppService</span></span>

* <span data-ttu-id="f138f-2432">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="f138f-2432">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f138f-2433">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="f138f-2433">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f138f-2434">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="f138f-2434">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f138f-2435">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="f138f-2435">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f138f-2436">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="f138f-2436">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f138f-2437">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f138f-2437">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f138f-2438">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="f138f-2438">support slot swap with preview</span></span>
* <span data-ttu-id="f138f-2439">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f138f-2439">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f138f-2440">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f138f-2440">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f138f-2441">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f138f-2441">CosmosDB</span></span>

* <span data-ttu-id="f138f-2442">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f138f-2442">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f138f-2443">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="f138f-2443">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f138f-2444">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="f138f-2444">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f138f-2445">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="f138f-2445">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f138f-2446">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f138f-2446">Data Lake Analytics</span></span>

* <span data-ttu-id="f138f-2447">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="f138f-2447">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f138f-2448">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="f138f-2448">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f138f-2449">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f138f-2449">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f138f-2450">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="f138f-2450">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f138f-2451">Table</span><span class="sxs-lookup"><span data-stu-id="f138f-2451">Table</span></span>
  * <span data-ttu-id="f138f-2452">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="f138f-2452">Table valued function</span></span>
  * <span data-ttu-id="f138f-2453">Sicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2453">View</span></span>
  * <span data-ttu-id="f138f-2454">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="f138f-2454">Table Statistics.</span></span> <span data-ttu-id="f138f-2455">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="f138f-2455">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f138f-2456">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f138f-2456">Data Lake Store</span></span>

* <span data-ttu-id="f138f-2457">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-2457">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f138f-2458">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f138f-2458">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f138f-2459">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="f138f-2459">missed help for access show.</span></span> <span data-ttu-id="f138f-2460">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f138f-2460">adding it.</span></span> <span data-ttu-id="f138f-2461">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f138f-2461">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f138f-2462">Suchen</span><span class="sxs-lookup"><span data-stu-id="f138f-2462">Find</span></span>

* <span data-ttu-id="f138f-2463">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="f138f-2463">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f138f-2464">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f138f-2464">KeyVault</span></span>

* <span data-ttu-id="f138f-2465">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="f138f-2465">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f138f-2466">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f138f-2466">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f138f-2467">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="f138f-2467">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f138f-2468">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="f138f-2468">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f138f-2469">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f138f-2469">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f138f-2470">Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-2470">Lab</span></span>

* <span data-ttu-id="f138f-2471">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="f138f-2471">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f138f-2472">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-2472">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f138f-2473">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="f138f-2473">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f138f-2474">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="f138f-2474">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f138f-2475">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="f138f-2475">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f138f-2476">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f138f-2476">Monitor</span></span>

* <span data-ttu-id="f138f-2477">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f138f-2477">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f138f-2478">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f138f-2478">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f138f-2479">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2479">Network</span></span>

* <span data-ttu-id="f138f-2480">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f138f-2480">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f138f-2481">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f138f-2481">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f138f-2482">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="f138f-2482">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f138f-2483">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="f138f-2483">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f138f-2484">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="f138f-2484">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f138f-2485">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="f138f-2485">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f138f-2486">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2486">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f138f-2487">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f138f-2487">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f138f-2488">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="f138f-2488">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f138f-2489">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="f138f-2489">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f138f-2490">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="f138f-2490">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f138f-2491">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f138f-2491">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f138f-2492">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="f138f-2492">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f138f-2493">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f138f-2493">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f138f-2494">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f138f-2494">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f138f-2495">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="f138f-2495">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f138f-2496">Profil</span><span class="sxs-lookup"><span data-stu-id="f138f-2496">Profile</span></span>

* <span data-ttu-id="f138f-2497">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f138f-2497">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f138f-2498">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f138f-2498">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f138f-2499">Redis</span><span class="sxs-lookup"><span data-stu-id="f138f-2499">Redis</span></span>

* <span data-ttu-id="f138f-2500">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="f138f-2500">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f138f-2501">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="f138f-2501">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f138f-2502">Resource</span><span class="sxs-lookup"><span data-stu-id="f138f-2502">Resource</span></span>

* <span data-ttu-id="f138f-2503">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f138f-2503">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f138f-2504">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f138f-2504">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f138f-2505">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f138f-2505">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f138f-2506">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="f138f-2506">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f138f-2507">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f138f-2507">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f138f-2508">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="f138f-2508">Add docs for az lock update.</span></span> <span data-ttu-id="f138f-2509">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f138f-2509">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f138f-2510">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="f138f-2510">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f138f-2511">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f138f-2511">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f138f-2512">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="f138f-2512">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f138f-2513">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f138f-2513">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f138f-2514">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f138f-2514">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f138f-2515">Rolle</span><span class="sxs-lookup"><span data-stu-id="f138f-2515">Role</span></span>

* <span data-ttu-id="f138f-2516">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f138f-2516">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f138f-2517">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f138f-2517">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f138f-2518">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f138f-2518">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f138f-2519">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="f138f-2519">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f138f-2520">SQL</span><span class="sxs-lookup"><span data-stu-id="f138f-2520">SQL</span></span>

* <span data-ttu-id="f138f-2521">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="f138f-2521">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f138f-2522">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f138f-2522">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f138f-2523">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2523">Storage</span></span>

* <span data-ttu-id="f138f-2524">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f138f-2524">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f138f-2525">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="f138f-2525">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f138f-2526">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="f138f-2526">Add support for large block blob upload</span></span>
* <span data-ttu-id="f138f-2527">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="f138f-2527">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2528">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2528">VM</span></span>

* <span data-ttu-id="f138f-2529">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="f138f-2529">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f138f-2530">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="f138f-2530">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f138f-2531">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f138f-2531">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f138f-2532">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f138f-2532">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f138f-2533">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="f138f-2533">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f138f-2534">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="f138f-2534">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f138f-2535">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f138f-2535">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f138f-2536">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2536">April 3, 2017</span></span>

<span data-ttu-id="f138f-2537">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f138f-2537">Version 2.0.2</span></span>

<span data-ttu-id="f138f-2538">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2538">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="f138f-2539">Core</span><span class="sxs-lookup"><span data-stu-id="f138f-2539">Core</span></span>

* <span data-ttu-id="f138f-2540">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="f138f-2540">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f138f-2541">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f138f-2541">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f138f-2542">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f138f-2542">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f138f-2543">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f138f-2543">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f138f-2544">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f138f-2544">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f138f-2545">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="f138f-2545">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f138f-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f138f-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f138f-2547">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2547">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f138f-2548">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="f138f-2548">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f138f-2549">ACS</span><span class="sxs-lookup"><span data-stu-id="f138f-2549">ACS</span></span>

* <span data-ttu-id="f138f-2550">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f138f-2550">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f138f-2551">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="f138f-2551">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f138f-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f138f-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f138f-2553">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="f138f-2553">Add support for windows clusters.</span></span> <span data-ttu-id="f138f-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f138f-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f138f-2555">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="f138f-2555">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f138f-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f138f-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f138f-2557">AppService</span><span class="sxs-lookup"><span data-stu-id="f138f-2557">AppService</span></span>

* <span data-ttu-id="f138f-2558">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f138f-2558">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f138f-2559">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f138f-2559">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f138f-2560">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f138f-2560">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f138f-2561">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f138f-2561">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f138f-2562">DataLake</span><span class="sxs-lookup"><span data-stu-id="f138f-2562">DataLake</span></span>

* <span data-ttu-id="f138f-2563">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2563">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f138f-2564">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="f138f-2564">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f138f-2565">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f138f-2565">DocuemntDB</span></span>

* <span data-ttu-id="f138f-2566">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f138f-2566">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f138f-2567">VM</span><span class="sxs-lookup"><span data-stu-id="f138f-2567">VM</span></span>

* <span data-ttu-id="f138f-2568">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f138f-2568">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f138f-2569">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f138f-2569">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f138f-2570">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f138f-2570">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f138f-2571">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f138f-2571">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f138f-2572">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f138f-2572">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f138f-2573">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="f138f-2573">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f138f-2574">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f138f-2574">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f138f-2575">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="f138f-2575">February 27, 2017</span></span>

<span data-ttu-id="f138f-2576">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f138f-2576">Version 2.0.0</span></span>

<span data-ttu-id="f138f-2577">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="f138f-2577">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f138f-2578">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="f138f-2578">Container Service (acs)</span></span>
- <span data-ttu-id="f138f-2579">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f138f-2579">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f138f-2580">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f138f-2580">Networking</span></span>
- <span data-ttu-id="f138f-2581">Storage</span><span class="sxs-lookup"><span data-stu-id="f138f-2581">Storage</span></span>

<span data-ttu-id="f138f-2582">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="f138f-2582">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f138f-2583">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="f138f-2583">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f138f-2584">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f138f-2584">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="f138f-2585">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="f138f-2585">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f138f-2586">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f138f-2586">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f138f-2587">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="f138f-2587">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f138f-2588">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f138f-2588">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f138f-2589">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="f138f-2589">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f138f-2590">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f138f-2590">Provide feedback from the command line with the `az feedback` command</span></span>


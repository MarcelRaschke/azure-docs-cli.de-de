---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/02/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 26757193628cff65603a04e440f9e2aa7bf5a248
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527301"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="44718-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="44718-103">Azure CLI release notes</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="44718-104">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="44718-104">July 2, 2019</span></span>

<span data-ttu-id="44718-105">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="44718-105">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="44718-106">Core</span><span class="sxs-lookup"><span data-stu-id="44718-106">Core</span></span>

* <span data-ttu-id="44718-107">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="44718-107">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="44718-108">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="44718-108">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="44718-109">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="44718-109">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="44718-110">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-110">ACR</span></span>

* <span data-ttu-id="44718-111">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-111">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-112">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-112">Appservice</span></span>

* <span data-ttu-id="44718-113">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="44718-113">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="44718-114">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-114">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="44718-115">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="44718-115">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="44718-116">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-116">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="44718-117">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="44718-117">Cosmos DB</span></span>

* <span data-ttu-id="44718-118">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-118">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="44718-119">DLS</span><span class="sxs-lookup"><span data-stu-id="44718-119">DLS</span></span>

* <span data-ttu-id="44718-120">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="44718-120">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="44718-121">Feedback</span><span class="sxs-lookup"><span data-stu-id="44718-121">Feedback</span></span>

* <span data-ttu-id="44718-122">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="44718-122">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-123">HDInsight</span></span>

* <span data-ttu-id="44718-124">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-124">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="44718-125">[BREAKING CHANGE] `--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="44718-125">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="44718-126">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-126">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="44718-127">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="44718-127">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="44718-128">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-128">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="44718-129">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-129">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="44718-130">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-130">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="44718-131">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="44718-131">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="44718-132">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-132">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="44718-133">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="44718-133">Managed Services</span></span>

* <span data-ttu-id="44718-134">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="44718-134">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="44718-135">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-135">Profile</span></span>
* <span data-ttu-id="44718-136">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="44718-136">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="44718-137">RBAC</span><span class="sxs-lookup"><span data-stu-id="44718-137">RBAC</span></span>

* <span data-ttu-id="44718-138">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-138">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="44718-139">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="44718-139">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="44718-140">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="44718-140">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="44718-141">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="44718-141">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-142">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-142">RDBMS</span></span>

* <span data-ttu-id="44718-143">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-143">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="44718-144">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-144">SQL</span></span>

* <span data-ttu-id="44718-145">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="44718-145">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-146">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-146">Storage</span></span>

* <span data-ttu-id="44718-147">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-147">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="44718-148">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-148">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="44718-149">VM</span><span class="sxs-lookup"><span data-stu-id="44718-149">VM</span></span>

* <span data-ttu-id="44718-150">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="44718-150">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="44718-151">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-151">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="44718-152">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="44718-152">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="44718-153">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-153">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="44718-154">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="44718-154">June 18, 2019</span></span>

<span data-ttu-id="44718-155">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="44718-155">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="44718-156">Core</span><span class="sxs-lookup"><span data-stu-id="44718-156">Core</span></span>

<span data-ttu-id="44718-157">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="44718-157">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="44718-158">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="44718-158">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="44718-159">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="44718-159">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="44718-160">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="44718-160">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="44718-161">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="44718-161">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="44718-162">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="44718-162">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="44718-163">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="44718-163">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="44718-164">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-164">ACR</span></span>
* <span data-ttu-id="44718-165">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-165">Added 'acr check-health' command</span></span>
* <span data-ttu-id="44718-166">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="44718-166">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="44718-167">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-167">ACS</span></span>
* <span data-ttu-id="44718-168">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="44718-168">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="44718-169">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-169">AMS</span></span>
* <span data-ttu-id="44718-170">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="44718-170">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-171">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-171">AppService</span></span>
* <span data-ttu-id="44718-172">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-172">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="44718-173">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-173">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="44718-174">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-174">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="44718-175">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-175">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="44718-176">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-176">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="44718-177">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-177">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="44718-178">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-178">Batch</span></span>
* <span data-ttu-id="44718-179">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="44718-179">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-180">Batch AI</span><span class="sxs-lookup"><span data-stu-id="44718-180">BatchAI</span></span>
* <span data-ttu-id="44718-181">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="44718-181">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-182">BotService</span><span class="sxs-lookup"><span data-stu-id="44718-182">BotService</span></span>
* <span data-ttu-id="44718-183">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-183">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-184">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-184">CosmosDB</span></span>
* <span data-ttu-id="44718-185">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="44718-185">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="44718-186">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="44718-186">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="44718-187">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-187">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="44718-188">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="44718-188">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="44718-189">EventGrid</span><span class="sxs-lookup"><span data-stu-id="44718-189">EventGrid</span></span>
* <span data-ttu-id="44718-190">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-190">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="44718-191">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-191">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="44718-192">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-192">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="44718-193">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-193">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="44718-194">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-194">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-195">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-195">HDInsight</span></span>
* <span data-ttu-id="44718-196">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-196">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="44718-197">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-197">IoT</span></span>
* <span data-ttu-id="44718-198">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-198">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="44718-199">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-199">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="44718-200">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-200">Network</span></span>
* <span data-ttu-id="44718-201">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-201">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="44718-202">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-202">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="44718-203">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="44718-203">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="44718-204">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-204">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="44718-205">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-205">Resource</span></span>
* <span data-ttu-id="44718-206">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-206">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="44718-207">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-207">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="44718-208">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="44718-208">ServiceBus</span></span>
* <span data-ttu-id="44718-209">Problem mit `servicebus topic create --max-size` behoben [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="44718-209">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="44718-210">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-210">SQL</span></span>
* <span data-ttu-id="44718-211">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="44718-211">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="44718-212">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-212">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="44718-213">SQLVm</span><span class="sxs-lookup"><span data-stu-id="44718-213">SQLVm</span></span>
* <span data-ttu-id="44718-214">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="44718-214">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="44718-215">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-215">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="44718-216">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-216">Storage</span></span>
* <span data-ttu-id="44718-217">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-217">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="44718-218">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="44718-218">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="44718-219">VM</span><span class="sxs-lookup"><span data-stu-id="44718-219">VM</span></span>
* <span data-ttu-id="44718-220">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-220">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="44718-221">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="44718-221">June 4, 2019</span></span>

<span data-ttu-id="44718-222">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="44718-222">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="44718-223">Core</span><span class="sxs-lookup"><span data-stu-id="44718-223">Core</span></span>
* <span data-ttu-id="44718-224">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="44718-224">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="44718-225">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-225">ACR</span></span>
* <span data-ttu-id="44718-226">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-226">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="44718-227">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-227">ACS</span></span>
* <span data-ttu-id="44718-228">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="44718-228">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="44718-229">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="44718-229">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="44718-230">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-230">Batch</span></span>
* <span data-ttu-id="44718-231">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="44718-231">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="44718-232">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-232">IoT</span></span>
* <span data-ttu-id="44718-233">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-233">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="44718-234">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-234">Network</span></span>
* <span data-ttu-id="44718-235">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-235">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="44718-236">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-236">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="44718-237">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-237">Resource</span></span>
* <span data-ttu-id="44718-238">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="44718-238">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="44718-239">Role</span><span class="sxs-lookup"><span data-stu-id="44718-239">Role</span></span>
* <span data-ttu-id="44718-240">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-240">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="44718-241">Compute</span><span class="sxs-lookup"><span data-stu-id="44718-241">Compute</span></span>
* <span data-ttu-id="44718-242">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="44718-242">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="44718-243">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="44718-243">May 21, 2019</span></span>

<span data-ttu-id="44718-244">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="44718-244">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="44718-245">Core</span><span class="sxs-lookup"><span data-stu-id="44718-245">Core</span></span>
* <span data-ttu-id="44718-246">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-246">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="44718-247">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="44718-247">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="44718-248">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="44718-248">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="44718-249">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-249">ACR</span></span>
* <span data-ttu-id="44718-250">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-250">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="44718-251">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-251">ACS</span></span>
* <span data-ttu-id="44718-252">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-252">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-253">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-253">AppService</span></span>
* <span data-ttu-id="44718-254">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-254">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="44718-255">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="44718-255">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="44718-256">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="44718-256">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="44718-257">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-257">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="44718-258">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="44718-258">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="44718-259">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="44718-259">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="44718-260">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="44718-260">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-261">BotService</span><span class="sxs-lookup"><span data-stu-id="44718-261">BotService</span></span>
* <span data-ttu-id="44718-262">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="44718-262">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="44718-263">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-263">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-264">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-264">Consumption</span></span>
* <span data-ttu-id="44718-265">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-265">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="44718-266">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-266">IoT</span></span>
* <span data-ttu-id="44718-267">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-267">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="44718-268">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-268">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="44718-270">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-270">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="44718-271">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="44718-271">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-272">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-272">RDBMS</span></span>
* <span data-ttu-id="44718-273">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-273">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="44718-274">RBAC</span><span class="sxs-lookup"><span data-stu-id="44718-274">RBAC</span></span>
* <span data-ttu-id="44718-275">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-275">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-276">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-276">Storage</span></span>
* <span data-ttu-id="44718-277">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-277">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="44718-278">Compute</span><span class="sxs-lookup"><span data-stu-id="44718-278">Compute</span></span>
* <span data-ttu-id="44718-279">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-279">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="44718-280">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="44718-280">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="44718-281">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="44718-281">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="44718-282">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="44718-282">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="44718-283">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="44718-283">May 6, 2019</span></span>

<span data-ttu-id="44718-284">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="44718-284">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="44718-285">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-285">ACS</span></span>
* <span data-ttu-id="44718-286">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-286">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="44718-287">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-287">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="44718-288">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-288">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="44718-289">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-289">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-290">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-290">Appservice</span></span>
* <span data-ttu-id="44718-291">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="44718-291">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="44718-292">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="44718-292">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="44718-293">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="44718-293">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="44718-294">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-294">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="44718-295">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-295">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="44718-296">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-296">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="44718-297">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-297">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="44718-298">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="44718-298">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="44718-299">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-299">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="44718-300">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-300">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="44718-301">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-301">Batch</span></span>
* <span data-ttu-id="44718-302">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-302">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-303">Botservice</span><span class="sxs-lookup"><span data-stu-id="44718-303">Botservice</span></span>
* <span data-ttu-id="44718-304">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="44718-304">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="44718-305">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-305">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="44718-306">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="44718-306">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="44718-307">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="44718-307">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="44718-308">[BREAKING CHANGE] `--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="44718-308">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="44718-309">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="44718-309">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="44718-310">[BREAKING CHANGE] `--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-310">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="44718-311">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-311">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="44718-312">[BREAKING CHANGE] `bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-312">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="44718-313">[BREAKING CHANGE] `bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="44718-313">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="44718-314">[BREAKING CHANGE] `bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="44718-314">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="44718-315">[BREAKING CHANGE] `--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="44718-315">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="44718-316">[BREAKING CHANGE] `Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-316">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="44718-317">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="44718-317">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="44718-318">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="44718-318">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="44718-319">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="44718-319">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="44718-320">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-320">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="44718-321">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="44718-321">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="44718-322">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="44718-322">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="44718-323">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-323">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="44718-324">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-324">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="44718-325">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="44718-325">Configure</span></span>
* <span data-ttu-id="44718-326">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-326">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="44718-327">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="44718-327">Eventhubs</span></span>
* <span data-ttu-id="44718-328">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-328">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="44718-329">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-329">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="44718-330">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-330">Network</span></span>
* <span data-ttu-id="44718-331">[BREAKING CHANGE] `--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="44718-331">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="44718-332">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="44718-332">Policy Insights</span></span>
* <span data-ttu-id="44718-333">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="44718-333">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="44718-334">Role</span><span class="sxs-lookup"><span data-stu-id="44718-334">Role</span></span>
* <span data-ttu-id="44718-335">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-335">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="44718-336">Service Bus</span><span class="sxs-lookup"><span data-stu-id="44718-336">Service Bus</span></span>
* <span data-ttu-id="44718-337">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-337">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="44718-338">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-338">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="44718-339">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="44718-339">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="44718-340">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-340">SQL</span></span>
* <span data-ttu-id="44718-341">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-341">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="44718-342">VM</span><span class="sxs-lookup"><span data-stu-id="44718-342">VM</span></span>
* <span data-ttu-id="44718-343">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="44718-343">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="44718-344">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="44718-344">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="44718-345">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-345">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="44718-346">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-346">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="44718-347">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-347">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="44718-348">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-348">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="44718-349">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="44718-349">April 23, 2019</span></span>

<span data-ttu-id="44718-350">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="44718-350">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="44718-351">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-351">ACS</span></span>
* <span data-ttu-id="44718-352">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="44718-352">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="44718-353">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-353">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="44718-354">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-354">AMS</span></span>
* <span data-ttu-id="44718-355">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="44718-355">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-356">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-356">AppService</span></span>
* <span data-ttu-id="44718-357">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-357">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="44718-358">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-358">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="44718-359">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="44718-359">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="44718-360">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="44718-360">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="44718-361">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="44718-361">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="44718-362">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-362">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="44718-363">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="44718-363">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="44718-364">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="44718-364">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="44718-365">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="44718-365">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="44718-366">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="44718-366">Deployment Manager</span></span>
* <span data-ttu-id="44718-367">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-367">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="44718-368">Labor</span><span class="sxs-lookup"><span data-stu-id="44718-368">Lab</span></span>
* <span data-ttu-id="44718-369">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="44718-369">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="44718-370">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-370">Network</span></span>
* <span data-ttu-id="44718-371">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-371">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="44718-372">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-372">Resource</span></span>
* <span data-ttu-id="44718-373">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-373">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="44718-374">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="44718-374">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="44718-375">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-375">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="44718-376">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="44718-376">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="44718-377">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-377">SQL</span></span>
* <span data-ttu-id="44718-378">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-378">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="44718-379">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="44718-379">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="44718-380">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-380">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="44718-381">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-381">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-382">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-382">Storage</span></span>
* <span data-ttu-id="44718-383">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-383">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-384">VM</span><span class="sxs-lookup"><span data-stu-id="44718-384">VM</span></span>
* <span data-ttu-id="44718-385">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-385">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="44718-386">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-386">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="44718-387">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="44718-387">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="44718-388">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="44718-388">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="44718-389">Core</span><span class="sxs-lookup"><span data-stu-id="44718-389">Core</span></span>
* <span data-ttu-id="44718-390">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-390">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="44718-391">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-391">ACR</span></span>
* <span data-ttu-id="44718-392">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-392">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="44718-393">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-393">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="44718-396">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-396">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="44718-397">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-397">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-398">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-398">AppService</span></span>
* <span data-ttu-id="44718-399">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-399">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="44718-400">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-400">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="44718-401">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-401">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="44718-402">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="44718-402">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="44718-403">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-403">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="44718-404">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-404">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="44718-405">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-405">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-406">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-406">CDN</span></span>
* <span data-ttu-id="44718-407">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="44718-407">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="44718-408">Feedback</span><span class="sxs-lookup"><span data-stu-id="44718-408">Feedback</span></span>
* <span data-ttu-id="44718-409">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="44718-409">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="44718-410">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="44718-410">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="44718-411">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="44718-411">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-412">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-412">Monitor</span></span>
* <span data-ttu-id="44718-413">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="44718-413">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="44718-414">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-414">Network</span></span>
* <span data-ttu-id="44718-415">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-415">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="44718-416">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-416">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="44718-417">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-417">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="44718-418">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="44718-418">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="44718-419">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="44718-419">PrivateDNS</span></span>
* <span data-ttu-id="44718-420">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-420">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="44718-421">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-421">Resource</span></span>
* <span data-ttu-id="44718-422">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-422">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="44718-423">Role</span><span class="sxs-lookup"><span data-stu-id="44718-423">Role</span></span>
* <span data-ttu-id="44718-424">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="44718-424">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="44718-425">[BREAKING CHANGE] `role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="44718-425">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="44718-426">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-426">SQL</span></span>
* <span data-ttu-id="44718-427">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-427">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="44718-428">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-428">Storage</span></span>
* <span data-ttu-id="44718-429">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-429">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="44718-430">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="44718-430">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="44718-431">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="44718-431">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="44718-432">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-432">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="44718-433">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="44718-433">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="44718-434">Core</span><span class="sxs-lookup"><span data-stu-id="44718-434">Core</span></span>
* <span data-ttu-id="44718-435">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="44718-435">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="44718-436">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="44718-436">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="44718-437">Cloud</span><span class="sxs-lookup"><span data-stu-id="44718-437">Cloud</span></span>
* <span data-ttu-id="44718-438">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-438">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="44718-439">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-439">ACR</span></span>
* <span data-ttu-id="44718-440">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-440">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="44718-441">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-441">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="44718-442">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-442">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="44718-443">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-443">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-444">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-444">AppService</span></span>
* <span data-ttu-id="44718-445">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-445">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="44718-446">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-446">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="44718-447">Bot Service</span><span class="sxs-lookup"><span data-stu-id="44718-447">BOT Service</span></span>
* <span data-ttu-id="44718-448">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="44718-448">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="44718-449">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="44718-449">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="44718-450">[BREAKING CHANGE] `--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="44718-450">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="44718-451">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-451">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-452">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-452">CDN</span></span>
* <span data-ttu-id="44718-453">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-453">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="44718-454">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-454">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="44718-455">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="44718-455">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="44718-456">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="44718-456">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-457">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="44718-457">Cosmosdb</span></span>
* <span data-ttu-id="44718-458">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-458">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="44718-459">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-459">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-460">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-460">Interactive</span></span>
* <span data-ttu-id="44718-461">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-461">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-462">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-462">Monitor</span></span>
* <span data-ttu-id="44718-463">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="44718-463">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="44718-464">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-464">Network</span></span>
* <span data-ttu-id="44718-465">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-465">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-466">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-466">Profile</span></span>
* <span data-ttu-id="44718-467">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-467">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="44718-468">Postgres</span><span class="sxs-lookup"><span data-stu-id="44718-468">Postgres</span></span> 
* <span data-ttu-id="44718-469">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-469">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="44718-470">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="44718-470">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="44718-471">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-471">Resource</span></span>
* <span data-ttu-id="44718-472">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="44718-472">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="44718-473">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-473">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="44718-474">Graph</span><span class="sxs-lookup"><span data-stu-id="44718-474">Graph</span></span>
* <span data-ttu-id="44718-475">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-475">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="44718-476">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-476">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="44718-477">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="44718-477">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="44718-478">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="44718-478">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="44718-479">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-479">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="44718-480">storage</span><span class="sxs-lookup"><span data-stu-id="44718-480">storage</span></span>
* <span data-ttu-id="44718-481">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-481">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="44718-482">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="44718-482">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="44718-483">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-483">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="44718-484">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="44718-484">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="44718-485">VM</span><span class="sxs-lookup"><span data-stu-id="44718-485">VM</span></span>
* <span data-ttu-id="44718-486">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-486">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="44718-487">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="44718-487">March 12, 2019</span></span>

<span data-ttu-id="44718-488">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="44718-488">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="44718-489">Core</span><span class="sxs-lookup"><span data-stu-id="44718-489">Core</span></span>

* <span data-ttu-id="44718-490">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-490">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="44718-491">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-491">ACR</span></span>

* <span data-ttu-id="44718-492">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-492">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="44718-493">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-493">ACS</span></span>

* <span data-ttu-id="44718-494">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="44718-494">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="44718-495">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-495">AppService</span></span>

* <span data-ttu-id="44718-496">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="44718-496">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="44718-497">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-497">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="44718-498">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="44718-498">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="44718-499">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="44718-499">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-500">Botservice</span><span class="sxs-lookup"><span data-stu-id="44718-500">Botservice</span></span>

* <span data-ttu-id="44718-501">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-501">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="44718-502">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-502">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="44718-503">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-503">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="44718-504">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="44718-504">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="44718-505">Container</span><span class="sxs-lookup"><span data-stu-id="44718-505">Container</span></span>

* <span data-ttu-id="44718-506">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-506">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="44718-507">EventHub</span><span class="sxs-lookup"><span data-stu-id="44718-507">EventHub</span></span>

* <span data-ttu-id="44718-508">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-508">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="44718-509">Suchen</span><span class="sxs-lookup"><span data-stu-id="44718-509">Find</span></span>

* <span data-ttu-id="44718-510">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="44718-510">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-511">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-511">HDInsight</span></span>

* <span data-ttu-id="44718-512">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-512">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="44718-513">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-513">Network</span></span>

* <span data-ttu-id="44718-514">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="44718-514">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-515">Rdbms</span><span class="sxs-lookup"><span data-stu-id="44718-515">Rdbms</span></span>

* <span data-ttu-id="44718-516">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="44718-516">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="44718-517">Role</span><span class="sxs-lookup"><span data-stu-id="44718-517">Role</span></span>

* <span data-ttu-id="44718-518">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="44718-518">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="44718-519">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="44718-519">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="44718-520">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="44718-520">Service Fabric</span></span>

* <span data-ttu-id="44718-521">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-521">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="44718-522">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="44718-522">February 26, 2019</span></span>

<span data-ttu-id="44718-523">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="44718-523">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="44718-524">Core</span><span class="sxs-lookup"><span data-stu-id="44718-524">Core</span></span>

* <span data-ttu-id="44718-525">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="44718-525">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="44718-526">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-526">ACR</span></span>

* <span data-ttu-id="44718-527">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-527">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="44718-528">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="44718-528">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="44718-529">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-529">ACS</span></span>

* <span data-ttu-id="44718-530">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-530">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-531">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-531">AppService</span></span>

* <span data-ttu-id="44718-532">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-532">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="44718-533">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-533">Batch</span></span>
* <span data-ttu-id="44718-534">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-534">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="44718-535">[BREAKING CHANGE] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-535">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="44718-536">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-536">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="44718-537">[BREAKING CHANGE] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="44718-537">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="44718-538">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-538">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="44718-539">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="44718-539">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-540">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-540">CosmosDB</span></span>

* <span data-ttu-id="44718-541">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-541">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="44718-542">Kusto</span><span class="sxs-lookup"><span data-stu-id="44718-542">Kusto</span></span>

* <span data-ttu-id="44718-543">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="44718-543">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="44718-544">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-544">Network</span></span>

* <span data-ttu-id="44718-545">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-545">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="44718-546">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-546">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="44718-547">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-547">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="44718-548">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-548">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="44718-549">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-549">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="44718-550">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-550">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="44718-551">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-551">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="44718-552">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-552">Resource</span></span>

* <span data-ttu-id="44718-553">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="44718-553">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="44718-554">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-554">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="44718-555">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-555">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="44718-556">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-556">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="44718-557">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-557">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="44718-558">Role</span><span class="sxs-lookup"><span data-stu-id="44718-558">Role</span></span>

* <span data-ttu-id="44718-559">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-559">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-560">VM</span><span class="sxs-lookup"><span data-stu-id="44718-560">VM</span></span>

* <span data-ttu-id="44718-561">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="44718-561">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="44718-562">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="44718-562">February 12, 2019</span></span>

<span data-ttu-id="44718-563">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="44718-563">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="44718-564">Core</span><span class="sxs-lookup"><span data-stu-id="44718-564">Core</span></span>

* <span data-ttu-id="44718-565">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="44718-565">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="44718-566">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-566">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="44718-567">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-567">ACR</span></span>
* <span data-ttu-id="44718-568">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-568">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="44718-569">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-569">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="44718-570">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-570">ACS</span></span>
* <span data-ttu-id="44718-571">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-571">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="44718-572">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-572">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="44718-573">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-573">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="44718-574">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-574">AMS</span></span>
* <span data-ttu-id="44718-575">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-575">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="44718-576">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-576">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-577">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-577">Appservice</span></span>
* <span data-ttu-id="44718-578">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-578">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="44718-579">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-579">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="44718-580">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="44718-580">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="44718-581">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-581">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="44718-582">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-582">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-583">Botservice</span><span class="sxs-lookup"><span data-stu-id="44718-583">Botservice</span></span>
* <span data-ttu-id="44718-584">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="44718-584">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="44718-585">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-585">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="44718-586">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-586">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="44718-587">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="44718-587">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="44718-588">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-588">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="44718-589">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="44718-589">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="44718-590">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="44718-590">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="44718-591">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-591">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="44718-592">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="44718-592">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="44718-593">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="44718-593">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="44718-594">Key Vault</span><span class="sxs-lookup"><span data-stu-id="44718-594">Key Vault</span></span>
* <span data-ttu-id="44718-595">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="44718-595">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-596">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-596">Monitor</span></span>
* <span data-ttu-id="44718-597">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="44718-597">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="44718-598">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-598">Network</span></span>
* <span data-ttu-id="44718-599">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="44718-599">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="44718-600">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="44718-600">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="44718-601">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="44718-601">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="44718-602">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-602">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="44718-603">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="44718-603">Policy Insights</span></span>
* <span data-ttu-id="44718-604">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="44718-604">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-605">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-605">RDBMS</span></span>
* <span data-ttu-id="44718-606">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="44718-606">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="44718-607">Redis</span><span class="sxs-lookup"><span data-stu-id="44718-607">Redis</span></span>
* <span data-ttu-id="44718-608">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-608">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="44718-609">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-609">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="44718-610">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-610">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="44718-611">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-611">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="44718-612">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-612">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="44718-613">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="44718-613">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="44718-614">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-614">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="44718-615">Role</span><span class="sxs-lookup"><span data-stu-id="44718-615">Role</span></span>
* <span data-ttu-id="44718-616">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="44718-616">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="44718-617">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="44718-617">SQL VM</span></span>
* <span data-ttu-id="44718-618">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-618">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="44718-619">VM</span><span class="sxs-lookup"><span data-stu-id="44718-619">VM</span></span>
* <span data-ttu-id="44718-620">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="44718-620">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="44718-621">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-621">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="44718-622">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="44718-622">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="44718-623">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="44718-623">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="44718-624">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="44718-624">January 31, 2019</span></span>

<span data-ttu-id="44718-625">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="44718-625">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="44718-626">Core</span><span class="sxs-lookup"><span data-stu-id="44718-626">Core</span></span>

* <span data-ttu-id="44718-627">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="44718-627">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="44718-628">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="44718-628">January 28, 2019</span></span>

<span data-ttu-id="44718-629">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="44718-629">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="44718-630">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-630">ACR</span></span>
* <span data-ttu-id="44718-631">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-631">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="44718-632">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-632">ACS</span></span>
* <span data-ttu-id="44718-633">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-633">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="44718-634">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-634">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="44718-635">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-635">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="44718-636">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-636">AMS</span></span>
* <span data-ttu-id="44718-637">[BREAKING CHANGE] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-637">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="44718-638">[BREAKING CHANGE] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-638">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-639">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-639">Appservice</span></span>
* <span data-ttu-id="44718-640">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-640">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="44718-641">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-641">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="44718-642">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-642">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="44718-643">Container</span><span class="sxs-lookup"><span data-stu-id="44718-643">Container</span></span>
* <span data-ttu-id="44718-644">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-644">Added `container start` command</span></span>
* <span data-ttu-id="44718-645">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="44718-645">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="44718-646">EventGrid</span><span class="sxs-lookup"><span data-stu-id="44718-646">EventGrid</span></span>
* <span data-ttu-id="44718-647">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-647">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="44718-648">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-648">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="44718-649">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="44718-649">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="44718-650">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="44718-650">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="44718-651">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="44718-651">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-652">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-652">HDInsight</span></span>
* <span data-ttu-id="44718-653">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-653">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="44718-654">[BREAKING CHANGE] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="44718-654">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="44718-655">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-655">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="44718-656">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-656">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="44718-657">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-657">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="44718-658">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-658">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="44718-659">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-659">IoT</span></span>
* <span data-ttu-id="44718-660">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-660">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="44718-661">Kusto</span><span class="sxs-lookup"><span data-stu-id="44718-661">Kusto</span></span>
* <span data-ttu-id="44718-662">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="44718-662">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-663">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-663">Monitor</span></span>
* <span data-ttu-id="44718-664">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="44718-664">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="44718-665">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-665">Profile</span></span>
* <span data-ttu-id="44718-666">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="44718-666">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="44718-667">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-667">Network</span></span>
* <span data-ttu-id="44718-668">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="44718-668">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="44718-669">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="44718-669">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="44718-670">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-670">Resource</span></span>
* <span data-ttu-id="44718-671">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-671">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="44718-672">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-672">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="44718-673">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="44718-673">SQL Virtual Machine</span></span>
* <span data-ttu-id="44718-674">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="44718-674">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="44718-675">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-675">Storage</span></span>
* <span data-ttu-id="44718-676">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="44718-676">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="44718-677">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="44718-677">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="44718-678">VM</span><span class="sxs-lookup"><span data-stu-id="44718-678">VM</span></span>
* <span data-ttu-id="44718-679">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="44718-679">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="44718-680">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-680">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="44718-681">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="44718-681">January 15, 2019</span></span>

<span data-ttu-id="44718-682">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="44718-682">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="44718-683">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-683">ACR</span></span>
* <span data-ttu-id="44718-684">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-684">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="44718-685">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-685">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="44718-686">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="44718-686">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="44718-687">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-687">ACS</span></span>
* <span data-ttu-id="44718-688">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-688">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-689">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-689">Appservice</span></span>
* <span data-ttu-id="44718-690">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="44718-690">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="44718-691">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="44718-691">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="44718-692">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="44718-692">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="44718-693">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-693">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-694">Botservice</span><span class="sxs-lookup"><span data-stu-id="44718-694">Botservice</span></span>
* <span data-ttu-id="44718-695">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-695">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="44718-696">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="44718-696">Configure</span></span>
* <span data-ttu-id="44718-697">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-697">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-698">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-698">CosmosDB</span></span>
* <span data-ttu-id="44718-699">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-699">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-700">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-700">HDInsight</span></span>
* <span data-ttu-id="44718-701">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-701">Added commands for managing applications</span></span>
* <span data-ttu-id="44718-702">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-702">Added commands for managing script actions</span></span>
* <span data-ttu-id="44718-703">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-703">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="44718-704">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-704">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="44718-705">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-705">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="44718-706">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-706">Network</span></span>
* <span data-ttu-id="44718-707">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-707">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="44718-708">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="44718-708">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="44718-709">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-709">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="44718-710">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="44718-710">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="44718-711">Role</span><span class="sxs-lookup"><span data-stu-id="44718-711">Role</span></span>
* <span data-ttu-id="44718-712">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="44718-712">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="44718-713">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="44718-713">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="44718-714">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="44718-714">Security</span></span>
* <span data-ttu-id="44718-715">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-715">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="44718-716">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-716">Storage</span></span>
* <span data-ttu-id="44718-717">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-717">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="44718-718">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="44718-718">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="44718-719">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-719">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="44718-720">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-720">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="44718-721">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-721">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="44718-722">VM</span><span class="sxs-lookup"><span data-stu-id="44718-722">VM</span></span>
* <span data-ttu-id="44718-723">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="44718-723">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="44718-724">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-724">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="44718-725">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-725">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="44718-726">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="44718-726">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="44718-727">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="44718-727">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="44718-728">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="44718-728">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="44718-729">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="44718-729">December 20, 2018</span></span>

<span data-ttu-id="44718-730">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="44718-730">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="44718-731">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-731">Appservice</span></span>
* <span data-ttu-id="44718-732">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-732">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="44718-733">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-733">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="44718-734">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-734">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="44718-735">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="44718-735">IoTCentral</span></span>
* <span data-ttu-id="44718-736">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="44718-736">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="44718-737">Role</span><span class="sxs-lookup"><span data-stu-id="44718-737">Role</span></span>
* <span data-ttu-id="44718-738">[BREAKING CHANGE] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="44718-738">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="44718-739">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-739">SQL</span></span>
* <span data-ttu-id="44718-740">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-740">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="44718-741">VM</span><span class="sxs-lookup"><span data-stu-id="44718-741">VM</span></span>
* <span data-ttu-id="44718-742">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-742">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="44718-743">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="44718-743">December 18, 2018</span></span>

<span data-ttu-id="44718-744">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="44718-744">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="44718-745">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-745">ACR</span></span>
* <span data-ttu-id="44718-746">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-746">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="44718-747">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="44718-747">Condensed the table layout for task list</span></span>
* <span data-ttu-id="44718-748">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-748">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="44718-749">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-749">ACS</span></span>
* <span data-ttu-id="44718-750">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-750">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="44718-751">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-751">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="44718-752">[VERALTET] `az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="44718-752">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="44718-753">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="44718-753">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="44718-754">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-754">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="44718-755">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-755">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-756">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-756">Appservice</span></span>
* <span data-ttu-id="44718-757">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-757">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="44718-758">Botservice</span><span class="sxs-lookup"><span data-stu-id="44718-758">Botservice</span></span>
* <span data-ttu-id="44718-759">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-759">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="44718-760">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="44718-760">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="44718-761">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="44718-761">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="44718-762">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="44718-762">Reduced Kudu network calls</span></span>
* <span data-ttu-id="44718-763">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="44718-763">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-764">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-764">Consumption</span></span>
* <span data-ttu-id="44718-765">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="44718-765">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-766">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-766">CosmosDB</span></span>
* <span data-ttu-id="44718-767">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-767">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="44718-768">Karten</span><span class="sxs-lookup"><span data-stu-id="44718-768">Maps</span></span>
* <span data-ttu-id="44718-769">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-769">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="44718-770">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-770">Network</span></span>
* <span data-ttu-id="44718-771">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-771">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="44718-772">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="44718-772">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="44718-773">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-773">Resource</span></span>
* <span data-ttu-id="44718-774">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-774">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="44718-775">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-775">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-776">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-776">Storage</span></span>
*  <span data-ttu-id="44718-777">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-777">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-778">VM</span><span class="sxs-lookup"><span data-stu-id="44718-778">VM</span></span>
* <span data-ttu-id="44718-779">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="44718-779">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="44718-780">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="44718-780">December 4, 2018</span></span>

<span data-ttu-id="44718-781">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="44718-781">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="44718-782">Core</span><span class="sxs-lookup"><span data-stu-id="44718-782">Core</span></span>
* <span data-ttu-id="44718-783">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-783">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="44718-784">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-784">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-785">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-785">Appservice</span></span>
* <span data-ttu-id="44718-786">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="44718-786">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="44718-787">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-787">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="44718-788">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-788">Network</span></span>
* <span data-ttu-id="44718-789">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-789">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="44718-790">Role</span><span class="sxs-lookup"><span data-stu-id="44718-790">Role</span></span>
* <span data-ttu-id="44718-791">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-791">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="44718-792">VM</span><span class="sxs-lookup"><span data-stu-id="44718-792">VM</span></span>
* <span data-ttu-id="44718-793">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-793">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="44718-794">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="44718-794">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="44718-795">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="44718-795">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="44718-796">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="44718-796">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="44718-797">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="44718-797">November 20, 2018</span></span>

<span data-ttu-id="44718-798">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="44718-798">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="44718-799">Core</span><span class="sxs-lookup"><span data-stu-id="44718-799">Core</span></span>
* <span data-ttu-id="44718-800">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-800">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="44718-801">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-801">ACR</span></span>
* <span data-ttu-id="44718-802">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-802">Added context token to task step</span></span>
* <span data-ttu-id="44718-803">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-803">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="44718-804">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-804">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-805">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-805">Appservice</span></span>
* <span data-ttu-id="44718-806">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-806">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="44718-807">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="44718-807">Updated the default `node_version`.</span></span> <span data-ttu-id="44718-808">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="44718-808">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="44718-809">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-809">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="44718-810">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="44718-810">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="44718-811">IotCentral</span><span class="sxs-lookup"><span data-stu-id="44718-811">IotCentral</span></span>
* <span data-ttu-id="44718-812">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-812">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-813">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-813">KeyVault</span></span>
* <span data-ttu-id="44718-814">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-814">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="44718-815">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-815">Network</span></span>
* <span data-ttu-id="44718-816">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-816">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="44718-817">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-817">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="44718-818">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-818">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="44718-819">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-819">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-820">Rdbms</span><span class="sxs-lookup"><span data-stu-id="44718-820">Rdbms</span></span>
* <span data-ttu-id="44718-821">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-821">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="44718-822">RBAC</span><span class="sxs-lookup"><span data-stu-id="44718-822">Rbac</span></span>
* <span data-ttu-id="44718-823">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-823">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="44718-824">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-824">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="44718-825">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-825">Storage</span></span>
* <span data-ttu-id="44718-826">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-826">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="44718-827">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="44718-827">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="44718-828">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="44718-828">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="44718-829">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="44718-829">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="44718-830">VM</span><span class="sxs-lookup"><span data-stu-id="44718-830">VM</span></span>
* <span data-ttu-id="44718-831">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-831">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="44718-832">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="44718-832">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="44718-833">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="44718-833">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="44718-834">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-834">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="44718-835">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-835">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="44718-836">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-836">Added `snapshot wait` command</span></span>
* <span data-ttu-id="44718-837">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-837">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="44718-838">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="44718-838">November 6, 2018</span></span>

<span data-ttu-id="44718-839">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="44718-839">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="44718-840">Core</span><span class="sxs-lookup"><span data-stu-id="44718-840">Core</span></span>
* <span data-ttu-id="44718-841">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-841">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="44718-842">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-842">ACR</span></span>
* <span data-ttu-id="44718-843">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-843">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="44718-844">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="44718-844">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="44718-845">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-845">ACS</span></span>
* <span data-ttu-id="44718-846">[BREAKING CHANGE] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="44718-846">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="44718-847">Advisor</span><span class="sxs-lookup"><span data-stu-id="44718-847">Advisor</span></span>
* <span data-ttu-id="44718-848">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="44718-848">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="44718-849">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-849">AMS</span></span>
* <span data-ttu-id="44718-850">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-850">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="44718-851">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-851">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="44718-852">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-852">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="44718-853">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="44718-853">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="44718-854">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-854">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="44718-855">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-855">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="44718-856">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-856">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="44718-857">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="44718-857">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="44718-858">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-858">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="44718-859">[BREAKING CHANGE] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-859">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="44718-860">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="44718-860">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="44718-861">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="44718-861">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="44718-862">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="44718-862">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="44718-863">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="44718-863">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="44718-864">[BREAKING CHANGE] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="44718-864">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="44718-865">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="44718-865">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="44718-866">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="44718-866">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-867">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-867">AppService</span></span>
* <span data-ttu-id="44718-868">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="44718-868">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="44718-869">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="44718-869">Configure</span></span>
* <span data-ttu-id="44718-870">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-870">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="44718-871">Container</span><span class="sxs-lookup"><span data-stu-id="44718-871">Container</span></span>
* <span data-ttu-id="44718-872">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="44718-872">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="44718-873">EventHub</span><span class="sxs-lookup"><span data-stu-id="44718-873">EventHub</span></span>
* <span data-ttu-id="44718-874">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-874">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-875">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-875">Interactive</span></span>
* <span data-ttu-id="44718-876">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-876">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-877">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-877">Monitor</span></span>
* <span data-ttu-id="44718-878">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-878">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="44718-879">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-879">Network</span></span>
* <span data-ttu-id="44718-880">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-880">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="44718-881">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="44718-881">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="44718-882">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="44718-882">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="44718-883">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-883">Profile</span></span>
* <span data-ttu-id="44718-884">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-884">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-885">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-885">RDBMS</span></span>
* <span data-ttu-id="44718-886">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-886">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="44718-887">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-887">Resource</span></span>
* <span data-ttu-id="44718-888">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-888">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="44718-889">Role</span><span class="sxs-lookup"><span data-stu-id="44718-889">Role</span></span>
* <span data-ttu-id="44718-890">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-890">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="44718-891">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="44718-891">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="44718-892">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-892">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="44718-893">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-893">Storage</span></span>
* <span data-ttu-id="44718-894">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="44718-894">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-895">VM</span><span class="sxs-lookup"><span data-stu-id="44718-895">VM</span></span>
* <span data-ttu-id="44718-896">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-896">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="44718-897">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="44718-897">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="44718-898">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-898">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="44718-899">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="44718-899">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="44718-900">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="44718-900">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="44718-901">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-901">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="44718-902">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="44718-902">October 23, 2018</span></span>

<span data-ttu-id="44718-903">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="44718-903">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="44718-904">Core</span><span class="sxs-lookup"><span data-stu-id="44718-904">Core</span></span>
* <span data-ttu-id="44718-905">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="44718-905">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="44718-906">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="44718-906">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="44718-907">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-907">ACR</span></span>
* <span data-ttu-id="44718-908">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="44718-908">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-909">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-909">CDN</span></span>
* <span data-ttu-id="44718-910">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="44718-910">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="44718-911">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="44718-911">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="44718-912">Container</span><span class="sxs-lookup"><span data-stu-id="44718-912">Container</span></span>
* <span data-ttu-id="44718-913">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-913">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="44718-914">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="44718-914">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="44718-915">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-915">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="44718-916">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="44718-916">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="44718-917">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="44718-917">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="44718-918">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="44718-918">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="44718-919">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-919">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-920">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-920">CosmosDB</span></span>
* <span data-ttu-id="44718-921">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-921">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-922">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-922">Interactive</span></span>
* <span data-ttu-id="44718-923">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="44718-923">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="44718-924">IoT Central</span><span class="sxs-lookup"><span data-stu-id="44718-924">IoT Central</span></span>
* <span data-ttu-id="44718-925">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-925">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="44718-926">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="44718-926">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-927">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-927">Monitor</span></span>
* <span data-ttu-id="44718-928">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="44718-928">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="44718-929">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-929">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="44718-930">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-930">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="44718-931">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-931">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="44718-932">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-932">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="44718-933">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="44718-933">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="44718-934">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="44718-934">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="44718-935">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-935">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="44718-936">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-936">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="44718-937">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-937">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="44718-938">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-938">Network</span></span>
* <span data-ttu-id="44718-939">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-939">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="44718-940">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-940">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="44718-941">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="44718-941">ServiceBus</span></span>
* <span data-ttu-id="44718-942">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-942">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="44718-943">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-943">SQL</span></span>
* <span data-ttu-id="44718-944">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="44718-944">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="44718-945">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-945">Storage</span></span>
* <span data-ttu-id="44718-946">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-946">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="44718-947">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-947">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="44718-948">VM</span><span class="sxs-lookup"><span data-stu-id="44718-948">VM</span></span>
* <span data-ttu-id="44718-949">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="44718-949">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="44718-950">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-950">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="44718-951">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-951">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="44718-952">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="44718-952">October 16, 2018</span></span>

<span data-ttu-id="44718-953">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="44718-953">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="44718-954">VM</span><span class="sxs-lookup"><span data-stu-id="44718-954">VM</span></span>
* <span data-ttu-id="44718-955">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="44718-955">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="44718-956">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="44718-956">October 9, 2018</span></span>

<span data-ttu-id="44718-957">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="44718-957">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="44718-958">Core</span><span class="sxs-lookup"><span data-stu-id="44718-958">Core</span></span>
* <span data-ttu-id="44718-959">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="44718-959">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="44718-960">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-960">ACR</span></span>
* <span data-ttu-id="44718-961">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-961">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="44718-962">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-962">ACS</span></span>
* <span data-ttu-id="44718-963">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="44718-963">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="44718-964">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="44718-964">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="44718-965">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="44718-965">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="44718-966">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="44718-966">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="44718-967">Container</span><span class="sxs-lookup"><span data-stu-id="44718-967">Container</span></span>
* <span data-ttu-id="44718-968">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="44718-968">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="44718-969">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-969">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="44718-970">Event Hub</span><span class="sxs-lookup"><span data-stu-id="44718-970">Event Hub</span></span>
* <span data-ttu-id="44718-971">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-971">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="44718-972">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-972">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="44718-973">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="44718-973">Extensions</span></span>
* <span data-ttu-id="44718-974">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="44718-974">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="44718-975">HDInsight</span><span class="sxs-lookup"><span data-stu-id="44718-975">HDInsight</span></span>
* <span data-ttu-id="44718-976">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-976">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="44718-977">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-977">IoT</span></span>
* <span data-ttu-id="44718-978">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-978">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-979">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-979">KeyVault</span></span>
* <span data-ttu-id="44718-980">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="44718-980">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="44718-981">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-981">Network</span></span>
* <span data-ttu-id="44718-982">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="44718-982">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="44718-983">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="44718-983">See #6052</span></span>
* <span data-ttu-id="44718-984">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="44718-984">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="44718-985">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="44718-985">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="44718-986">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-986">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="44718-987">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-987">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="44718-988">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="44718-988">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="44718-989">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-989">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="44718-990">Role</span><span class="sxs-lookup"><span data-stu-id="44718-990">Role</span></span>
* <span data-ttu-id="44718-991">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-991">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="44718-992">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-992">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="44718-993">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="44718-993">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="44718-994">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="44718-994">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="44718-995">Service Bus</span><span class="sxs-lookup"><span data-stu-id="44718-995">Service Bus</span></span>
* <span data-ttu-id="44718-996">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-996">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="44718-997">VM</span><span class="sxs-lookup"><span data-stu-id="44718-997">VM</span></span>
* <span data-ttu-id="44718-998">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-998">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="44718-999">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="44718-999">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="44718-1000">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1000">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="44718-1001">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1001">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="44718-1002">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1002">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="44718-1003">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1003">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="44718-1004">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1004">September 21, 2018</span></span>

<span data-ttu-id="44718-1005">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="44718-1005">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1006">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1006">ACR</span></span>
* <span data-ttu-id="44718-1007">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1007">Added ACR Task commands</span></span>
* <span data-ttu-id="44718-1008">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1008">Added quick run command</span></span>
* <span data-ttu-id="44718-1009">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1009">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="44718-1010">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1010">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="44718-1011">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1011">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="44718-1012">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1012">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1013">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1013">ACS</span></span>
* <span data-ttu-id="44718-1014">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1014">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="44718-1015">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1015">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1016">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1016">AppService</span></span>

* <span data-ttu-id="44718-1017">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="44718-1017">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="44718-1018">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1018">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="44718-1019">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1019">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="44718-1020">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1020">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1021">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1021">Batch</span></span>
* <span data-ttu-id="44718-1022">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1022">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="44718-1023">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1023">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="44718-1024">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1024">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="44718-1025">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1025">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="44718-1026">Batch KI</span><span class="sxs-lookup"><span data-stu-id="44718-1026">Batch AI</span></span> 
* <span data-ttu-id="44718-1027">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1027">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="44718-1028">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="44718-1028">Cognitive Services</span></span>
* <span data-ttu-id="44718-1029">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1029">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="44718-1030">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1030">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="44718-1031">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1031">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="44718-1032">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1032">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="44718-1033">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1033">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="44718-1034">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="44718-1034">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="44718-1035">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1035">Container</span></span>
* <span data-ttu-id="44718-1036">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1036">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="44718-1037">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1037">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="44718-1038">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1038">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="44718-1039">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1039">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="44718-1040">Data Lake</span><span class="sxs-lookup"><span data-stu-id="44718-1040">Datalake</span></span>
* <span data-ttu-id="44718-1041">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1041">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="44718-1042">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="44718-1042">Interactive Shell</span></span>
* <span data-ttu-id="44718-1043">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1043">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="44718-1044">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1044">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="44718-1045">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1045">IoT</span></span>
* <span data-ttu-id="44718-1046">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1046">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="44718-1047">Key Vault</span><span class="sxs-lookup"><span data-stu-id="44718-1047">Key Vault</span></span>
* <span data-ttu-id="44718-1048">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1048">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="44718-1049">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1049">Network</span></span>
* <span data-ttu-id="44718-1050">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1050">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="44718-1051">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1051">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="44718-1052">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1052">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="44718-1053">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-1053">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="44718-1054">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1054">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="44718-1055">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1055">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="44718-1056">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-1056">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="44718-1057">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="44718-1057">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="44718-1058">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1058">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="44718-1059">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1059">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="44718-1060">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1060">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="44718-1061">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1061">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="44718-1062">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1062">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="44718-1063">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="44718-1063">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="44718-1064">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1064">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="44718-1065">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="44718-1065">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="44718-1066">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1066">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="44718-1067">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1067">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-1068">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-1068">RDBMS</span></span>
* <span data-ttu-id="44718-1069">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1069">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="44718-1070">Reservierung</span><span class="sxs-lookup"><span data-stu-id="44718-1070">Reservation</span></span>
* <span data-ttu-id="44718-1071">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1071">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="44718-1072">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1072">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="44718-1073">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="44718-1073">Manage App</span></span>
* <span data-ttu-id="44718-1074">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="44718-1074">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="44718-1075">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="44718-1075">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="44718-1076">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1076">Role</span></span>
* <span data-ttu-id="44718-1077">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1077">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="44718-1078">SignalR</span><span class="sxs-lookup"><span data-stu-id="44718-1078">SignalR</span></span>
* <span data-ttu-id="44718-1079">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1079">First release</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1080">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1080">Storage</span></span>
* <span data-ttu-id="44718-1081">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1081">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="44718-1082">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1082">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1083">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1083">VM</span></span>
* <span data-ttu-id="44718-1084">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="44718-1084">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="44718-1085">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1085">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="44718-1086">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1086">August 28, 2018</span></span>

<span data-ttu-id="44718-1087">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="44718-1087">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="44718-1088">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1088">Core</span></span>

* <span data-ttu-id="44718-1089">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-1089">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="44718-1090">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1090">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1091">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1091">ACR</span></span>

* <span data-ttu-id="44718-1092">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1092">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="44718-1093">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="44718-1093">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1094">ACS</span></span>

* <span data-ttu-id="44718-1095">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="44718-1095">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="44718-1096">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="44718-1096">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1097">AppService</span></span>

* <span data-ttu-id="44718-1098">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1098">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="44718-1099">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1099">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="44718-1100">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1100">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="44718-1101">Backup</span><span class="sxs-lookup"><span data-stu-id="44718-1101">Backup</span></span>

* <span data-ttu-id="44718-1102">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1102">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="44718-1103">Botdienst</span><span class="sxs-lookup"><span data-stu-id="44718-1103">Bot Service</span></span>

* <span data-ttu-id="44718-1104">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="44718-1104">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="44718-1105">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="44718-1105">Cognitive Services</span></span>

* <span data-ttu-id="44718-1106">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="44718-1106">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="44718-1107">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1107">IoT</span></span>

* <span data-ttu-id="44718-1108">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1108">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1109">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1109">Monitor</span></span>

* <span data-ttu-id="44718-1110">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1110">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="44718-1111">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1111">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="44718-1112">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1112">Network</span></span>

* <span data-ttu-id="44718-1113">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1113">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1114">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1114">Resource</span></span>

* <span data-ttu-id="44718-1115">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1115">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1116">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1116">Storage</span></span>

* <span data-ttu-id="44718-1117">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1117">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1118">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1118">VM</span></span>

* <span data-ttu-id="44718-1119">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="44718-1119">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="44718-1120">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="44718-1120">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="44718-1121">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1121">Auguest 14, 2018</span></span>

<span data-ttu-id="44718-1122">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="44718-1122">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="44718-1123">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1123">Core</span></span>

* <span data-ttu-id="44718-1124">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1124">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="44718-1125">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1125">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="44718-1126">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="44718-1126">Telemetry</span></span>

* <span data-ttu-id="44718-1127">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="44718-1127">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1128">ACR</span></span>

* <span data-ttu-id="44718-1129">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1129">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="44718-1130">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="44718-1130">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1131">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1131">ACS</span></span>

* <span data-ttu-id="44718-1132">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1132">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="44718-1133">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="44718-1133">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="44718-1134">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="44718-1134">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="44718-1135">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="44718-1135">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="44718-1136">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="44718-1136">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="44718-1137">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1137">AppService</span></span>

* <span data-ttu-id="44718-1138">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="44718-1138">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="44718-1139">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1139">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-1140">Batch AI</span><span class="sxs-lookup"><span data-stu-id="44718-1140">BatchAI</span></span>

* <span data-ttu-id="44718-1141">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="44718-1141">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="44718-1142">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1142">Container</span></span>

* <span data-ttu-id="44718-1143">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1143">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="44718-1144">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1144">IoT</span></span>

* <span data-ttu-id="44718-1145">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1145">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="44718-1146">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="44718-1146">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="44718-1147">Iot Central</span><span class="sxs-lookup"><span data-stu-id="44718-1147">Iot Central</span></span>

* <span data-ttu-id="44718-1148">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-1148">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-1149">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-1149">KeyVault</span></span>


* <span data-ttu-id="44718-1150">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1150">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="44718-1151">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1151">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="44718-1152">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1152">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="44718-1153">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1153">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="44718-1154">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1154">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="44718-1155">Relay</span><span class="sxs-lookup"><span data-stu-id="44718-1155">Relay</span></span>

* <span data-ttu-id="44718-1156">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1156">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1157">Sql</span><span class="sxs-lookup"><span data-stu-id="44718-1157">Sql</span></span>

* <span data-ttu-id="44718-1158">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1158">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1159">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1159">Storage</span></span>

* <span data-ttu-id="44718-1160">[BREAKING CHANGE] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="44718-1160">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="44718-1161">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="44718-1161">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="44718-1162">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1162">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="44718-1163">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="44718-1163">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="44718-1164">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="44718-1164">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1165">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1165">VM</span></span>

* <span data-ttu-id="44718-1166">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1166">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="44718-1167">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1167">July 31, 2018</span></span>

<span data-ttu-id="44718-1168">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="44718-1168">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1169">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1169">ACR</span></span>

* <span data-ttu-id="44718-1170">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1170">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="44718-1171">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1171">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1172">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1172">ACS</span></span>

* <span data-ttu-id="44718-1173">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1173">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1174">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1174">Batch</span></span>

* <span data-ttu-id="44718-1175">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="44718-1175">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="44718-1176">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1176">Container</span></span>

* <span data-ttu-id="44718-1177">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1177">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="44718-1178">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1178">Network</span></span>

* <span data-ttu-id="44718-1179">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1179">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="44718-1180">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1180">Resource</span></span>

* <span data-ttu-id="44718-1181">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="44718-1181">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="44718-1182">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="44718-1182">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="44718-1183">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1183">Role</span></span>

* <span data-ttu-id="44718-1184">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1184">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="44718-1185">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="44718-1185">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="44718-1186">Suchen,</span><span class="sxs-lookup"><span data-stu-id="44718-1186">Search</span></span>

* <span data-ttu-id="44718-1187">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1187">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="44718-1188">Service Bus</span><span class="sxs-lookup"><span data-stu-id="44718-1188">Service Bus</span></span>

* <span data-ttu-id="44718-1189">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="44718-1189">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="44718-1190">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1190">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="44718-1191">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="44718-1191">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="44718-1192">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="44718-1192">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1193">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1193">Storage</span></span>

* <span data-ttu-id="44718-1194">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1194">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="44718-1195">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="44718-1195">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1196">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1196">VM</span></span>

* <span data-ttu-id="44718-1197">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1197">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="44718-1198">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1198">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="44718-1199">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1199">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="44718-1200">[BREAKING CHANGE] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="44718-1200">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="44718-1201">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1201">July 18, 2018</span></span>

<span data-ttu-id="44718-1202">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="44718-1202">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="44718-1203">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1203">Core</span></span>

* <span data-ttu-id="44718-1204">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1204">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="44718-1205">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1205">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="44718-1206">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="44718-1206">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1207">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1207">ACR</span></span>

* <span data-ttu-id="44718-1208">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1208">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="44718-1209">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1209">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="44718-1210">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-1210">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="44718-1211">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1211">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1212">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1212">ACS</span></span>

* <span data-ttu-id="44718-1213">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="44718-1213">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1214">AppService</span></span>

* <span data-ttu-id="44718-1215">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1215">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1216">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1216">Batch</span></span>

* <span data-ttu-id="44718-1217">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="44718-1217">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="44718-1218">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1218">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="44718-1219">Batch KI</span><span class="sxs-lookup"><span data-stu-id="44718-1219">Batch AI</span></span>

* <span data-ttu-id="44718-1220">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1220">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="44718-1221">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1221">Container</span></span>

* <span data-ttu-id="44718-1222">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1222">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="44718-1223">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1223">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="44718-1224">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1224">Network</span></span>

* <span data-ttu-id="44718-1225">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1225">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="44718-1226">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1226">Added `network nic wait`</span></span>
* <span data-ttu-id="44718-1227">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1227">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="44718-1228">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="44718-1228">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="44718-1229">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1229">Resource</span></span>

* <span data-ttu-id="44718-1230">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1230">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="44718-1231">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1231">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="44718-1232">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1232">Added `deployment wait` command</span></span>
* <span data-ttu-id="44718-1233">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1233">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1234">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1234">SQL</span></span>

* <span data-ttu-id="44718-1235">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1235">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="44718-1236">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="44718-1236">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="44718-1237">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1237">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1238">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1238">Storage</span></span>

* <span data-ttu-id="44718-1239">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1239">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1240">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1240">VM</span></span>

* <span data-ttu-id="44718-1241">[BREAKING CHANGE] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1241">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="44718-1242">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1242">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="44718-1243">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1243">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="44718-1244">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1244">July 3, 2018</span></span>

<span data-ttu-id="44718-1245">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="44718-1245">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="44718-1246">AKS</span><span class="sxs-lookup"><span data-stu-id="44718-1246">AKS</span></span>

* <span data-ttu-id="44718-1247">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1247">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="44718-1248">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1248">July 3, 2018</span></span>

<span data-ttu-id="44718-1249">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="44718-1249">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="44718-1250">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1250">Core</span></span>

* <span data-ttu-id="44718-1251">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1251">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1252">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1252">ACR</span></span>

* <span data-ttu-id="44718-1253">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1253">Added polling build status</span></span>
* <span data-ttu-id="44718-1254">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1254">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="44718-1255">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1255">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1256">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1256">ACS</span></span>

* <span data-ttu-id="44718-1257">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="44718-1257">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="44718-1258">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="44718-1258">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="44718-1259">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="44718-1259">Updated options for `aks browse` command.</span></span> <span data-ttu-id="44718-1260">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1260">Added `--listen-port` support</span></span>
* <span data-ttu-id="44718-1261">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="44718-1261">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="44718-1262">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="44718-1262">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="44718-1263">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1263">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1264">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1264">AppService</span></span>

* <span data-ttu-id="44718-1265">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1265">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="44718-1266">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1266">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="44718-1267">Backup</span><span class="sxs-lookup"><span data-stu-id="44718-1267">Backup</span></span>

* <span data-ttu-id="44718-1268">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1268">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-1269">Batch AI</span><span class="sxs-lookup"><span data-stu-id="44718-1269">BatchAI</span></span>

* <span data-ttu-id="44718-1270">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1270">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="44718-1271">Cloud</span><span class="sxs-lookup"><span data-stu-id="44718-1271">Cloud</span></span>

* <span data-ttu-id="44718-1272">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1272">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="44718-1273">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1273">Container</span></span>

* <span data-ttu-id="44718-1274">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1274">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="44718-1275">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1275">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="44718-1276">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1276">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1277">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1277">Extension</span></span>

* <span data-ttu-id="44718-1278">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="44718-1278">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="44718-1279">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1279">Network</span></span>

* <span data-ttu-id="44718-1280">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="44718-1280">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-1281">Rdbms</span><span class="sxs-lookup"><span data-stu-id="44718-1281">Rdbms</span></span>

* <span data-ttu-id="44718-1282">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1282">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1283">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1283">Resource</span></span>

* <span data-ttu-id="44718-1284">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1284">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1285">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1285">VM</span></span>

* <span data-ttu-id="44718-1286">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1286">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="44718-1287">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1287">June 25, 2018</span></span>

<span data-ttu-id="44718-1288">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="44718-1288">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="44718-1289">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="44718-1289">CLI</span></span>

* <span data-ttu-id="44718-1290">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="44718-1290">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="44718-1291">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1291">June 19, 2018</span></span>

<span data-ttu-id="44718-1292">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="44718-1292">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="44718-1293">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1293">Core</span></span>

* <span data-ttu-id="44718-1294">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1294">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1295">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1295">ACR</span></span>

* <span data-ttu-id="44718-1296">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1296">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="44718-1297">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="44718-1297">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1298">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1298">ACS</span></span>

* <span data-ttu-id="44718-1299">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="44718-1299">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="44718-1300">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1300">Added `--update` support</span></span>
* <span data-ttu-id="44718-1301">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1301">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="44718-1302">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-1302">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="44718-1303">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1303">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="44718-1304">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="44718-1304">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="44718-1305">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1305">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="44718-1306">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1306">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1307">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1307">AppService</span></span>

* <span data-ttu-id="44718-1308">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1308">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="44718-1309">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1309">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1310">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1310">Batch</span></span>

* <span data-ttu-id="44718-1311">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1311">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="44718-1312">Batch KI</span><span class="sxs-lookup"><span data-stu-id="44718-1312">Batch AI</span></span>

* <span data-ttu-id="44718-1313">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1313">Added support for workspaces.</span></span> <span data-ttu-id="44718-1314">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="44718-1314">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="44718-1315">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1315">Added support for experiments.</span></span> <span data-ttu-id="44718-1316">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="44718-1316">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="44718-1317">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="44718-1317">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="44718-1318">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1318">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="44718-1319">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="44718-1319">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="44718-1320">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1320">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="44718-1321">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-1321">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="44718-1322">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-1322">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="44718-1323">[BREAKING CHANGE] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1323">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="44718-1324">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="44718-1324">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="44718-1325">[BREAKING CHANGE] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1325">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="44718-1326">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="44718-1326">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="44718-1327">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1327">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="44718-1328">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="44718-1328">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="44718-1329">[BREAKING CHANGE] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1329">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="44718-1330">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="44718-1330">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="44718-1331">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1331">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="44718-1332">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1332">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="44718-1333">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1333">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="44718-1334">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1334">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="44718-1335">Karten</span><span class="sxs-lookup"><span data-stu-id="44718-1335">Maps</span></span>

* <span data-ttu-id="44718-1336">[BREAKING CHANGE] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="44718-1336">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="44718-1337">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1337">Network</span></span>

* <span data-ttu-id="44718-1338">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="44718-1338">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="44718-1339">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="44718-1339">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="44718-1340">#6502</span><span class="sxs-lookup"><span data-stu-id="44718-1340">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="44718-1341">Reservations</span><span class="sxs-lookup"><span data-stu-id="44718-1341">Reservations</span></span>

* <span data-ttu-id="44718-1342">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1342">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="44718-1343">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1343">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="44718-1344">[BREAKING CHANGE] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1344">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="44718-1345">[BREAKING CHANGE] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1345">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="44718-1346">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1346">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="44718-1347">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1347">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="44718-1348">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1348">Role</span></span>

* <span data-ttu-id="44718-1349">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1349">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1350">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1350">SQL</span></span>

* <span data-ttu-id="44718-1351">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="44718-1351">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1352">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1352">Storage</span></span>

* <span data-ttu-id="44718-1353">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1353">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1354">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1354">VM</span></span>

* <span data-ttu-id="44718-1355">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="44718-1355">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="44718-1356">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1356">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="44718-1357">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="44718-1357">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="44718-1358">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1358">June 13, 2018</span></span>

<span data-ttu-id="44718-1359">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="44718-1359">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="44718-1360">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1360">Core</span></span>

* <span data-ttu-id="44718-1361">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="44718-1361">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="44718-1362">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1362">June 13, 2018</span></span>

<span data-ttu-id="44718-1363">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="44718-1363">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="44718-1364">AKS</span><span class="sxs-lookup"><span data-stu-id="44718-1364">AKS</span></span>

* <span data-ttu-id="44718-1365">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1365">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="44718-1366">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1366">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="44718-1367">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1367">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="44718-1368">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1368">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="44718-1369">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1369">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1370">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1370">AppService</span></span>

* <span data-ttu-id="44718-1371">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1371">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="44718-1372">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1372">June 5, 2018</span></span>

<span data-ttu-id="44718-1373">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="44718-1373">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1374">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1374">Interactive</span></span>

* <span data-ttu-id="44718-1375">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1375">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="44718-1376">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1376">June 5, 2018</span></span>

<span data-ttu-id="44718-1377">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="44718-1377">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="44718-1378">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1378">Core</span></span>

* <span data-ttu-id="44718-1379">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1379">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="44718-1380">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="44718-1380">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1381">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1381">ACR</span></span>

* <span data-ttu-id="44718-1382">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1382">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="44718-1383">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1383">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="44718-1384">AKS</span><span class="sxs-lookup"><span data-stu-id="44718-1384">AKS</span></span>

* <span data-ttu-id="44718-1385">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="44718-1385">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1386">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1386">Batch</span></span>

* <span data-ttu-id="44718-1387">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="44718-1387">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="44718-1388">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1388">IOT</span></span>

* <span data-ttu-id="44718-1389">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1389">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="44718-1390">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1390">Network</span></span>

* <span data-ttu-id="44718-1391">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="44718-1391">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="44718-1392">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="44718-1392">Policy Insights</span></span>

* <span data-ttu-id="44718-1393">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1393">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="44718-1394">ARM</span><span class="sxs-lookup"><span data-stu-id="44718-1394">ARM</span></span>

* <span data-ttu-id="44718-1395">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1395">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1396">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1396">SQL</span></span>

* <span data-ttu-id="44718-1397">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-1397">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="44718-1398">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-1398">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="44718-1399">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1399">Storage</span></span>

* <span data-ttu-id="44718-1400">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="44718-1400">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1401">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1401">VM</span></span>

* <span data-ttu-id="44718-1402">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-1402">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="44718-1403">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1403">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="44718-1404">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1404">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="44718-1405">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1405">May 22, 2018</span></span>

<span data-ttu-id="44718-1406">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="44718-1406">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="44718-1407">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1407">Core</span></span>

* <span data-ttu-id="44718-1408">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1408">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1409">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1409">ACS</span></span>

* <span data-ttu-id="44718-1410">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1410">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="44718-1411">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1411">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1412">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1412">AppService</span></span>

* <span data-ttu-id="44718-1413">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="44718-1413">Improved generic update commands</span></span>
* <span data-ttu-id="44718-1414">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1414">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="44718-1415">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1415">Container</span></span>

* <span data-ttu-id="44718-1416">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1416">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="44718-1417">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1417">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1418">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1418">Extension</span></span>

* <span data-ttu-id="44718-1419">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="44718-1419">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1420">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1420">Interactive</span></span>

* <span data-ttu-id="44718-1421">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="44718-1421">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="44718-1422">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="44718-1422">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-1423">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-1423">KeyVault</span></span>

* <span data-ttu-id="44718-1424">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="44718-1424">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="44718-1425">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1425">Network</span></span>

* <span data-ttu-id="44718-1426">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="44718-1426">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="44718-1427">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="44718-1427">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1428">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1428">SQL</span></span>

* <span data-ttu-id="44718-1429">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="44718-1429">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="44718-1430">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1430">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="44718-1431">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1431">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="44718-1432">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="44718-1432">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="44718-1433">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="44718-1433">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="44718-1434">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="44718-1434">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="44718-1435">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="44718-1435">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="44718-1436">`edition`.</span><span class="sxs-lookup"><span data-stu-id="44718-1436">`edition`.</span></span> <span data-ttu-id="44718-1437">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="44718-1437">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="44718-1438">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="44718-1438">`elasticPoolName`.</span></span> <span data-ttu-id="44718-1439">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="44718-1439">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="44718-1440">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="44718-1440">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="44718-1441">`edition`.</span><span class="sxs-lookup"><span data-stu-id="44718-1441">`edition`.</span></span> <span data-ttu-id="44718-1442">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="44718-1442">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="44718-1443">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="44718-1443">`dtu`.</span></span> <span data-ttu-id="44718-1444">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="44718-1444">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="44718-1445">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="44718-1445">`databaseDtuMin`.</span></span> <span data-ttu-id="44718-1446">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="44718-1446">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="44718-1447">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="44718-1447">`databaseDtuMax`.</span></span> <span data-ttu-id="44718-1448">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="44718-1448">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="44718-1449">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1449">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="44718-1450">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1450">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1451">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1451">Storage</span></span>

* <span data-ttu-id="44718-1452">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1452">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="44718-1453">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1453">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1454">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1454">VM</span></span>

* <span data-ttu-id="44718-1455">[BREAKING CHANGE] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1455">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="44718-1456">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="44718-1456">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="44718-1457">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1457">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="44718-1458">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1458">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="44718-1459">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1459">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="44718-1460">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1460">May 7, 2018</span></span>

<span data-ttu-id="44718-1461">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="44718-1461">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="44718-1462">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1462">Core</span></span>

* <span data-ttu-id="44718-1463">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="44718-1463">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="44718-1464">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1464">Added limited support for positional arguments</span></span>
* <span data-ttu-id="44718-1465">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-1465">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="44718-1466">#5591</span><span class="sxs-lookup"><span data-stu-id="44718-1466">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="44718-1467">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1467">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="44718-1468">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="44718-1468">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="44718-1469">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="44718-1469">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="44718-1470">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="44718-1470">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="44718-1471">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1471">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1472">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1472">ACR</span></span>

* <span data-ttu-id="44718-1473">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1473">Added ACR Build commands</span></span>
* <span data-ttu-id="44718-1474">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1474">Improved resource not found error messages</span></span>
* <span data-ttu-id="44718-1475">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="44718-1475">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="44718-1476">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="44718-1476">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="44718-1477">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="44718-1477">Improved repository commands error messages</span></span>
* <span data-ttu-id="44718-1478">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1478">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1479">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1479">ACS</span></span>

* <span data-ttu-id="44718-1480">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="44718-1480">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="44718-1481">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="44718-1481">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="44718-1482">AMS</span><span class="sxs-lookup"><span data-stu-id="44718-1482">AMS</span></span>

* <span data-ttu-id="44718-1483">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="44718-1483">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1484">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1484">Appservice</span></span>

* <span data-ttu-id="44718-1485">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="44718-1485">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="44718-1486">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1486">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="44718-1487">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1487">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="44718-1488">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1488">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="44718-1489">Batch KI</span><span class="sxs-lookup"><span data-stu-id="44718-1489">Batch AI</span></span>

* <span data-ttu-id="44718-1490">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="44718-1490">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="44718-1491">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="44718-1491">Cognitive Services</span></span>

* <span data-ttu-id="44718-1492">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="44718-1492">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-1493">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-1493">Consumption</span></span>

* <span data-ttu-id="44718-1494">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1494">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="44718-1495">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1495">Container</span></span>

* <span data-ttu-id="44718-1496">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="44718-1496">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="44718-1497">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="44718-1497">Cosmos DB</span></span>

* <span data-ttu-id="44718-1498">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="44718-1498">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="44718-1499">DMS</span><span class="sxs-lookup"><span data-stu-id="44718-1499">DMS</span></span>

* <span data-ttu-id="44718-1500">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44718-1500">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1501">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1501">Extension</span></span>

* <span data-ttu-id="44718-1502">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1502">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1503">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1503">Interactive</span></span>

* <span data-ttu-id="44718-1504">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="44718-1504">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="44718-1505">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="44718-1505">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="44718-1506">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1506">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="44718-1507">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1507">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="44718-1508">Labor</span><span class="sxs-lookup"><span data-stu-id="44718-1508">Lab</span></span>

* <span data-ttu-id="44718-1509">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1509">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="44718-1510">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1510">Network</span></span>

* <span data-ttu-id="44718-1511">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="44718-1511">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="44718-1512">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1512">Profile</span></span>

* <span data-ttu-id="44718-1513">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1513">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="44718-1514">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="44718-1514">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="44718-1515">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1515">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="44718-1516">Redis</span><span class="sxs-lookup"><span data-stu-id="44718-1516">Redis</span></span>

* <span data-ttu-id="44718-1517">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="44718-1517">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="44718-1518">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1518">Deprecated `redis list-all`.</span></span> <span data-ttu-id="44718-1519">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="44718-1519">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="44718-1520">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="44718-1520">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="44718-1521">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1521">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="44718-1522">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1522">Role</span></span>

* <span data-ttu-id="44718-1523">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1523">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1524">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1524">Storage</span></span>

* <span data-ttu-id="44718-1525">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="44718-1525">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="44718-1526">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="44718-1526">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="44718-1527">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="44718-1527">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="44718-1528">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="44718-1528">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="44718-1529">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="44718-1529">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1530">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1530">VM</span></span>

* <span data-ttu-id="44718-1531">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1531">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="44718-1532">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1532">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="44718-1533">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="44718-1533">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="44718-1534">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1534">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="44718-1535">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="44718-1535">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="44718-1536">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1536">Added write accelerator support</span></span>
* <span data-ttu-id="44718-1537">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1537">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="44718-1538">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="44718-1538">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="44718-1539">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="44718-1539">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="44718-1540">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1540">April 10, 2018</span></span>

<span data-ttu-id="44718-1541">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="44718-1541">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1542">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1542">ACR</span></span>

* <span data-ttu-id="44718-1543">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="44718-1543">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1544">ACS</span></span>

* <span data-ttu-id="44718-1545">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1545">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1546">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1546">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="44718-1548">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1548">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-1549">Batch AI</span><span class="sxs-lookup"><span data-stu-id="44718-1549">BatchAI</span></span>

* <span data-ttu-id="44718-1550">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1550">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="44718-1551">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="44718-1551">Job level mounting</span></span>
  - <span data-ttu-id="44718-1552">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="44718-1552">Environment variables with secret values</span></span>
  - <span data-ttu-id="44718-1553">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="44718-1553">Performance counters settings</span></span>
  - <span data-ttu-id="44718-1554">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="44718-1554">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="44718-1555">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="44718-1555">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="44718-1556">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="44718-1556">Usage and limits reporting</span></span>
  - <span data-ttu-id="44718-1557">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="44718-1557">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="44718-1558">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="44718-1558">Support for custom images</span></span>
  - <span data-ttu-id="44718-1559">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1559">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="44718-1560">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="44718-1560">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="44718-1561">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="44718-1561">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="44718-1562">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="44718-1562">National clouds are supported</span></span>
* <span data-ttu-id="44718-1563">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1563">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="44718-1564">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="44718-1564">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="44718-1565">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1565">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="44718-1566">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="44718-1566">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="44718-1567">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="44718-1567">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="44718-1568">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="44718-1568">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="44718-1569">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="44718-1569">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="44718-1570">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1570">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="44718-1571">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="44718-1571">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="44718-1572">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1572">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="44718-1573">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="44718-1573">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="44718-1574">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="44718-1574">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="44718-1575">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="44718-1575">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="44718-1576">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="44718-1576">Billing</span></span>

* <span data-ttu-id="44718-1577">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1577">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-1578">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-1578">Consumption</span></span>

* <span data-ttu-id="44718-1579">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1579">Added `marketplace` commands</span></span>
* <span data-ttu-id="44718-1580">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1580">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="44718-1581">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1581">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="44718-1582">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1582">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="44718-1583">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1583">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="44718-1584">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1584">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="44718-1585">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1585">Container</span></span>

* <span data-ttu-id="44718-1586">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1586">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="44718-1587">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="44718-1587">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1588">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1588">Extension</span></span>

* <span data-ttu-id="44718-1589">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1589">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1590">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1590">Interactive</span></span>

* <span data-ttu-id="44718-1591">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="44718-1591">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="44718-1592">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1592">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="44718-1593">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1593">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="44718-1594">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1594">Network</span></span>

* <span data-ttu-id="44718-1595">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="44718-1595">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="44718-1596">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1596">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="44718-1597">#4910</span><span class="sxs-lookup"><span data-stu-id="44718-1597">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="44718-1598">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1598">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="44718-1599">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1599">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="44718-1600">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1600">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="44718-1601">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1601">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="44718-1602">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1602">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-1603">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1603">Profile</span></span>

* <span data-ttu-id="44718-1604">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1604">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="44718-1605">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1605">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-1606">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-1606">RDBMS</span></span>

* <span data-ttu-id="44718-1607">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1607">Added `georestore` command</span></span>
* <span data-ttu-id="44718-1608">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1608">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1609">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1609">Resource</span></span>

* <span data-ttu-id="44718-1610">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1610">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="44718-1611">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1611">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1612">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1612">SQL</span></span>

* <span data-ttu-id="44718-1613">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1613">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1614">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1614">Storage</span></span>

* <span data-ttu-id="44718-1615">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1615">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1616">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1616">VM</span></span>

* <span data-ttu-id="44718-1617">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1617">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="44718-1618">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="44718-1618">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="44718-1620">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1620">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="44718-1621">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="44718-1621">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="44718-1622">#5718</span><span class="sxs-lookup"><span data-stu-id="44718-1622">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="44718-1623">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="44718-1623">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="44718-1624">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1624">March 27, 2018</span></span>

<span data-ttu-id="44718-1625">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="44718-1625">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="44718-1626">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1626">Core</span></span>

* <span data-ttu-id="44718-1627">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="44718-1627">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1628">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1628">ACS</span></span>

* <span data-ttu-id="44718-1629">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="44718-1629">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1630">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1630">Appservice</span></span>

* <span data-ttu-id="44718-1631">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1631">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="44718-1632">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1632">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="44718-1633">Backup</span><span class="sxs-lookup"><span data-stu-id="44718-1633">Backup</span></span>

* <span data-ttu-id="44718-1634">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1634">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="44718-1635">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="44718-1635">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="44718-1636">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="44718-1636">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="44718-1637">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="44718-1637">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="44718-1638">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1638">Container</span></span>

* <span data-ttu-id="44718-1639">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1639">Added `container exec` command.</span></span> <span data-ttu-id="44718-1640">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="44718-1640">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="44718-1641">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="44718-1641">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1642">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1642">Extension</span></span>

* <span data-ttu-id="44718-1643">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="44718-1643">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="44718-1644">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-1644">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="44718-1645">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-1645">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1646">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1646">Interactive</span></span>

* <span data-ttu-id="44718-1647">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="44718-1647">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="44718-1648">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1648">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="44718-1649">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="44718-1649">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="44718-1650">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="44718-1650">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="44718-1651">Labor</span><span class="sxs-lookup"><span data-stu-id="44718-1651">Lab</span></span>

* <span data-ttu-id="44718-1652">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1652">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1653">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1653">Monitor</span></span>

* <span data-ttu-id="44718-1654">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="44718-1654">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="44718-1655">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="44718-1655">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="44718-1656">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="44718-1656">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="44718-1657">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1657">Network</span></span>

* <span data-ttu-id="44718-1658">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1658">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="44718-1659">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1659">Profile</span></span>

* <span data-ttu-id="44718-1660">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1660">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-1661">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-1661">RDBMS</span></span>

* <span data-ttu-id="44718-1662">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1662">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1663">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1663">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="44718-1665">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1665">Role</span></span>

* <span data-ttu-id="44718-1666">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1666">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="44718-1667">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="44718-1667">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="44718-1668">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1668">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="44718-1669">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1669">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="44718-1670">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1670">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1671">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1671">Storage</span></span>

* <span data-ttu-id="44718-1672">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1672">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="44718-1673">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="44718-1673">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1674">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1674">VM</span></span>

* <span data-ttu-id="44718-1675">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1675">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="44718-1676">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1676">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="44718-1677">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="44718-1677">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="44718-1678">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="44718-1678">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="44718-1679">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1679">March 13, 2018</span></span>

<span data-ttu-id="44718-1680">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="44718-1680">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1681">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1681">ACR</span></span>

* <span data-ttu-id="44718-1682">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1682">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="44718-1683">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1683">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="44718-1684">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1684">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1685">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1685">ACS</span></span>

* <span data-ttu-id="44718-1686">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1686">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="44718-1687">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1687">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="44718-1688">Advisor</span><span class="sxs-lookup"><span data-stu-id="44718-1688">Advisor</span></span>

* <span data-ttu-id="44718-1689">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1689">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="44718-1690">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1690">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="44718-1691">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1691">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="44718-1692">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1692">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="44718-1693">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1693">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1694">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1694">Appservice</span></span>

* <span data-ttu-id="44718-1695">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1695">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="44718-1696">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1696">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="44718-1697">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="44718-1697">Eventhubs</span></span>

* <span data-ttu-id="44718-1698">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1698">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1699">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1699">Extension</span></span>

* <span data-ttu-id="44718-1700">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="44718-1700">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1701">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1701">Interactive</span></span>

* <span data-ttu-id="44718-1702">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="44718-1702">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="44718-1703">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="44718-1703">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="44718-1704">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="44718-1704">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="44718-1705">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1705">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1706">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1706">Monitor</span></span>

* <span data-ttu-id="44718-1707">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1707">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="44718-1708">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1708">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="44718-1709">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1709">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="44718-1710">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1710">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="44718-1711">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1711">Network</span></span>

* <span data-ttu-id="44718-1712">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1712">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="44718-1713">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="44718-1713">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="44718-1714">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1714">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="44718-1715">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1715">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-1716">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1716">Profile</span></span>

* <span data-ttu-id="44718-1717">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1717">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="44718-1718">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1718">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-1719">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-1719">RDBMS</span></span>

* <span data-ttu-id="44718-1720">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1720">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="44718-1721">Service Bus</span><span class="sxs-lookup"><span data-stu-id="44718-1721">Service Bus</span></span>

* <span data-ttu-id="44718-1722">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1722">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1723">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1723">Storage</span></span>

* <span data-ttu-id="44718-1724">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="44718-1724">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="44718-1725">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="44718-1725">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1726">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1726">VM</span></span>

* <span data-ttu-id="44718-1727">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="44718-1727">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="44718-1728">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="44718-1728">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="44718-1729">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1729">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="44718-1730">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1730">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="44718-1731">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1731">February 27, 2018</span></span>

<span data-ttu-id="44718-1732">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="44718-1732">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="44718-1733">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1733">Core</span></span>

* <span data-ttu-id="44718-1734">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="44718-1734">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="44718-1735">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1735">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="44718-1736">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1736">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1737">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1737">ACS</span></span>

* <span data-ttu-id="44718-1738">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-1738">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="44718-1739">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="44718-1739">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="44718-1740">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1740">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="44718-1741">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1741">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1742">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1742">Appservice</span></span>

* <span data-ttu-id="44718-1743">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="44718-1743">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="44718-1744">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="44718-1744">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="44718-1745">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="44718-1745">Cognitive Services</span></span>

* <span data-ttu-id="44718-1746">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1746">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-1747">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-1747">Consumption</span></span>

* <span data-ttu-id="44718-1748">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1748">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="44718-1749">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1749">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="44718-1750">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1750">Container</span></span>

* <span data-ttu-id="44718-1751">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="44718-1751">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="44718-1752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1752">Network</span></span>

* <span data-ttu-id="44718-1753">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="44718-1753">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1754">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1754">Resource</span></span>

* <span data-ttu-id="44718-1755">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="44718-1755">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="44718-1756">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1756">Role</span></span>

* <span data-ttu-id="44718-1757">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1757">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1758">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1758">SQL</span></span>

* <span data-ttu-id="44718-1759">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="44718-1759">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1760">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1760">Storage</span></span>

* <span data-ttu-id="44718-1761">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-1761">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1762">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1762">VM</span></span>

* <span data-ttu-id="44718-1763">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1763">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="44718-1764">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1764">February 13, 2018</span></span>

<span data-ttu-id="44718-1765">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="44718-1765">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="44718-1766">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1766">Core</span></span>

* <span data-ttu-id="44718-1767">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1767">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1768">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1768">ACS</span></span>

* <span data-ttu-id="44718-1769">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-1769">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="44718-1770">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1770">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="44718-1771">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1771">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="44718-1772">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-1772">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="44718-1773">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1773">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="44718-1774">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1774">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="44718-1775">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="44718-1775">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="44718-1776">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="44718-1776">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1777">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1777">Appservice</span></span>

* <span data-ttu-id="44718-1778">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="44718-1778">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="44718-1779">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1779">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-1780">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-1780">CDN</span></span>

* <span data-ttu-id="44718-1781">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1781">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="44718-1782">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1782">Container</span></span>

* <span data-ttu-id="44718-1783">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1783">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="44718-1784">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1784">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-1785">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-1785">CosmosDB</span></span>

* <span data-ttu-id="44718-1786">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1786">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="44718-1787">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-1787">Extension</span></span>

* <span data-ttu-id="44718-1788">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1788">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="44718-1789">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1789">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="44718-1790">Feedback</span><span class="sxs-lookup"><span data-stu-id="44718-1790">Feedback</span></span>

* <span data-ttu-id="44718-1791">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1791">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1792">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1792">Interactive</span></span>

* <span data-ttu-id="44718-1793">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="44718-1793">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="44718-1794">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1794">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="44718-1795">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1795">IoT</span></span>

* <span data-ttu-id="44718-1796">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="44718-1796">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="44718-1797">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="44718-1797">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="44718-1798">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1798">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="44718-1799">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1799">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1800">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1800">Monitor</span></span>

* <span data-ttu-id="44718-1801">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1801">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="44718-1802">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1802">Network</span></span>

* <span data-ttu-id="44718-1803">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="44718-1803">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="44718-1804">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1804">Profile</span></span>

* <span data-ttu-id="44718-1805">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="44718-1805">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1806">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1806">Resource</span></span>

* <span data-ttu-id="44718-1807">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1807">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="44718-1808">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1808">Role</span></span>

* <span data-ttu-id="44718-1809">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1809">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1810">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1810">SQL</span></span>

* <span data-ttu-id="44718-1811">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1811">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="44718-1812">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1812">Added `sql db rename`</span></span>
* <span data-ttu-id="44718-1813">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1813">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1814">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1814">Storage</span></span>

* <span data-ttu-id="44718-1815">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1815">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1816">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1816">VM</span></span>

* <span data-ttu-id="44718-1817">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1817">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="44718-1818">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1818">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="44718-1819">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="44718-1819">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="44718-1820">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1820">January 31, 2018</span></span>

<span data-ttu-id="44718-1821">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="44718-1821">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="44718-1822">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1822">Core</span></span>

* <span data-ttu-id="44718-1823">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1823">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="44718-1824">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1824">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="44718-1825">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="44718-1825">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="44718-1826">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="44718-1826">Use `--verbose` to see</span></span>
* <span data-ttu-id="44718-1827">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1827">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1828">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1828">ACS</span></span>

* <span data-ttu-id="44718-1829">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="44718-1829">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="44718-1830">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1830">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1831">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1831">Appservice</span></span>

* <span data-ttu-id="44718-1832">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="44718-1832">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="44718-1833">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1833">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-1834">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-1834">CDN</span></span>

* <span data-ttu-id="44718-1835">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1835">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-1836">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-1836">CosmosDB</span></span>

* <span data-ttu-id="44718-1837">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1837">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1838">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1838">Interactive</span></span>

* <span data-ttu-id="44718-1839">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1839">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="44718-1840">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1840">Network</span></span>

* <span data-ttu-id="44718-1841">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1841">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="44718-1842">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="44718-1842">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="44718-1843">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1843">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="44718-1844">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1844">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="44718-1845">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1845">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="44718-1846">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="44718-1846">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="44718-1847">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1847">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="44718-1848">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1848">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="44718-1849">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1849">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="44718-1850">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="44718-1850">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="44718-1851">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1851">Profile</span></span>

* <span data-ttu-id="44718-1852">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1852">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1853">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1853">Resource</span></span>

* <span data-ttu-id="44718-1854">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="44718-1854">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1855">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1855">Storage</span></span>

* <span data-ttu-id="44718-1856">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1856">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="44718-1857">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1857">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="44718-1858">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="44718-1858">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="44718-1859">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1859">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="44718-1860">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="44718-1860">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1861">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1861">VM</span></span>

* <span data-ttu-id="44718-1862">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-1862">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="44718-1863">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="44718-1863">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="44718-1864">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1864">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="44718-1865">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1865">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="44718-1866">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="44718-1866">January 17, 2018</span></span>

<span data-ttu-id="44718-1867">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="44718-1867">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1868">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1868">ACR</span></span>

* <span data-ttu-id="44718-1869">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1869">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="44718-1870">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="44718-1870">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1871">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1871">ACS</span></span>

* <span data-ttu-id="44718-1872">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1872">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="44718-1873">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1873">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1874">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1874">Appservice</span></span>

* <span data-ttu-id="44718-1875">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="44718-1875">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="44718-1876">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1876">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="44718-1877">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1877">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="44718-1878">Backup</span><span class="sxs-lookup"><span data-stu-id="44718-1878">Backup</span></span>

* <span data-ttu-id="44718-1879">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="44718-1879">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="44718-1880">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1880">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="44718-1881">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="44718-1881">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="44718-1882">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-1882">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="44718-1883">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="44718-1883">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1884">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1884">Batch</span></span>

* <span data-ttu-id="44718-1885">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="44718-1885">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="44718-1886">Cloud</span><span class="sxs-lookup"><span data-stu-id="44718-1886">Cloud</span></span>

* <span data-ttu-id="44718-1887">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="44718-1887">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-1888">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-1888">Consumption</span></span>

* <span data-ttu-id="44718-1889">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="44718-1889">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="44718-1890">Event Grid</span><span class="sxs-lookup"><span data-stu-id="44718-1890">Event Grid</span></span>

* <span data-ttu-id="44718-1891">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="44718-1891">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="44718-1892">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="44718-1892">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="44718-1893">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1893">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="44718-1894">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="44718-1894">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="44718-1895">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1895">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="44718-1896">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1896">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="44718-1897">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1897">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="44718-1898">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1898">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-1899">Interactive</span><span class="sxs-lookup"><span data-stu-id="44718-1899">Interactive</span></span>

* <span data-ttu-id="44718-1900">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-1900">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="44718-1901">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1901">Fixed errors on startup</span></span>
* <span data-ttu-id="44718-1902">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-1902">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="44718-1903">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-1903">IoT</span></span>

* <span data-ttu-id="44718-1904">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1904">Added support for device provisioning service</span></span>
* <span data-ttu-id="44718-1905">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1905">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="44718-1906">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="44718-1906">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1907">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1907">Monitor</span></span>

* <span data-ttu-id="44718-1908">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1908">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="44718-1909">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44718-1909">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="44718-1910">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1910">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="44718-1911">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1911">Network</span></span>

* <span data-ttu-id="44718-1912">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-1912">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="44718-1913">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1913">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-1914">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-1914">Profile</span></span>

* <span data-ttu-id="44718-1915">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1915">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="44718-1916">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1916">Role</span></span>

* <span data-ttu-id="44718-1917">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="44718-1917">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="44718-1918">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="44718-1918">Service Fabric</span></span>

* <span data-ttu-id="44718-1919">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1919">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="44718-1920">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1920">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1921">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1921">VM</span></span>

* <span data-ttu-id="44718-1922">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="44718-1922">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="44718-1923">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1923">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="44718-1924">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="44718-1924">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="44718-1925">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1925">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="44718-1926">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1926">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="44718-1927">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1927">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="44718-1928">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1928">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="44718-1929">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1929">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="44718-1930">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="44718-1930">December 19, 2017</span></span>

<span data-ttu-id="44718-1931">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="44718-1931">Version 2.0.23</span></span>

* <span data-ttu-id="44718-1932">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1932">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="44718-1933">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1933">Container</span></span>

* <span data-ttu-id="44718-1934">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="44718-1934">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="44718-1935">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-1935">Network</span></span>

* <span data-ttu-id="44718-1936">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1936">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="44718-1937">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1937">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-1938">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-1938">Storage</span></span>

* <span data-ttu-id="44718-1939">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1939">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1940">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1940">VM</span></span>

* <span data-ttu-id="44718-1941">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1941">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="44718-1942">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="44718-1942">December 5, 2017</span></span>

<span data-ttu-id="44718-1943">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="44718-1943">Version 2.0.22</span></span>

* <span data-ttu-id="44718-1944">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-1944">Removed `az component` commands.</span></span> <span data-ttu-id="44718-1945">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="44718-1945">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="44718-1946">Core</span><span class="sxs-lookup"><span data-stu-id="44718-1946">Core</span></span>
* <span data-ttu-id="44718-1947">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-1947">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="44718-1948">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="44718-1948">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="44718-1949">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1949">ACS</span></span>

* <span data-ttu-id="44718-1950">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1950">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="44718-1951">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="44718-1951">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="44718-1952">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="44718-1952">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="44718-1953">Advisor</span><span class="sxs-lookup"><span data-stu-id="44718-1953">Advisor</span></span>

* <span data-ttu-id="44718-1954">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-1954">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1955">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1955">Appservice</span></span>

* <span data-ttu-id="44718-1956">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="44718-1956">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="44718-1957">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="44718-1957">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="44718-1958">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1958">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="44718-1959">Nutzung</span><span class="sxs-lookup"><span data-stu-id="44718-1959">Consumption</span></span>

* <span data-ttu-id="44718-1960">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1960">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="44718-1961">Container</span><span class="sxs-lookup"><span data-stu-id="44718-1961">Container</span></span>

* <span data-ttu-id="44718-1962">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="44718-1962">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-1963">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-1963">Monitor</span></span>

* <span data-ttu-id="44718-1964">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1964">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="44718-1965">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-1965">Resource</span></span>

* <span data-ttu-id="44718-1966">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1966">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="44718-1967">Role</span><span class="sxs-lookup"><span data-stu-id="44718-1967">Role</span></span>

* <span data-ttu-id="44718-1968">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1968">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="44718-1969">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1969">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="44718-1970">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="44718-1970">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="44718-1971">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-1971">SQL</span></span>

* <span data-ttu-id="44718-1972">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1972">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="44718-1973">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-1973">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="44718-1974">VM</span><span class="sxs-lookup"><span data-stu-id="44718-1974">VM</span></span>

* <span data-ttu-id="44718-1975">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1975">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="44718-1976">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="44718-1976">November 14, 2017</span></span>

<span data-ttu-id="44718-1977">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="44718-1977">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="44718-1978">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-1978">ACR</span></span>

* <span data-ttu-id="44718-1979">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1979">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="44718-1980">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-1980">ACS</span></span>

* <span data-ttu-id="44718-1981">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1981">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="44718-1982">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="44718-1982">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="44718-1983">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="44718-1983">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="44718-1984">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1984">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="44718-1985">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1985">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-1986">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-1986">Appservice</span></span>

* <span data-ttu-id="44718-1987">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1987">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="44718-1988">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1988">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="44718-1989">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-1989">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="44718-1990">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-1990">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="44718-1991">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1991">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="44718-1992">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="44718-1992">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="44718-1993">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-1993">Batch</span></span>

* <span data-ttu-id="44718-1994">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="44718-1994">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-1995">BatchAI</span><span class="sxs-lookup"><span data-stu-id="44718-1995">Batchai</span></span>

* <span data-ttu-id="44718-1996">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1996">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="44718-1997">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1997">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="44718-1998">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-1998">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="44718-1999">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-1999">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="44718-2000">Cloud</span><span class="sxs-lookup"><span data-stu-id="44718-2000">Cloud</span></span>

* <span data-ttu-id="44718-2001">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="44718-2001">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="44718-2002">Container</span><span class="sxs-lookup"><span data-stu-id="44718-2002">Container</span></span>

* <span data-ttu-id="44718-2003">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2003">Added support to open multiple ports</span></span>
* <span data-ttu-id="44718-2004">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2004">Added container group restart policy</span></span>
* <span data-ttu-id="44718-2005">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2005">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="44718-2006">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-2006">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="44718-2007">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="44718-2007">Data Lake Analytics</span></span>

* <span data-ttu-id="44718-2008">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="44718-2008">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="44718-2009">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="44718-2009">Data Lake Store</span></span>

* <span data-ttu-id="44718-2010">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="44718-2010">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="44718-2011">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-2011">Extension</span></span>

* <span data-ttu-id="44718-2012">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-2012">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="44718-2013">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="44718-2013">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="44718-2014">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-2014">IoT</span></span>

* <span data-ttu-id="44718-2015">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2015">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-2016">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-2016">Monitor</span></span>

* <span data-ttu-id="44718-2017">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2017">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="44718-2018">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2018">Network</span></span>

* <span data-ttu-id="44718-2019">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2019">Added support for CAA DNS records</span></span>
* <span data-ttu-id="44718-2020">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-2020">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="44718-2021">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="44718-2021">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="44718-2022">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2022">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="44718-2023">Reservations</span><span class="sxs-lookup"><span data-stu-id="44718-2023">Reservations</span></span>

* <span data-ttu-id="44718-2024">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="44718-2024">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2025">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2025">Resource</span></span>

* <span data-ttu-id="44718-2026">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2026">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2027">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-2027">SQL</span></span>

* <span data-ttu-id="44718-2028">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2028">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2029">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2029">Storage</span></span>

* <span data-ttu-id="44718-2030">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="44718-2030">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="44718-2031">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="44718-2031">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="44718-2032">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="44718-2032">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="44718-2033">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2033">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="44718-2034">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2034">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="44718-2035">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2035">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="44718-2036">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2036">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2037">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2037">VM</span></span>

* <span data-ttu-id="44718-2038">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="44718-2038">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="44718-2039">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2039">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="44718-2040">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="44718-2040">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="44718-2041">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2041">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="44718-2042">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2042">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="44718-2043">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2043">October 24, 2017</span></span>

<span data-ttu-id="44718-2044">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="44718-2044">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="44718-2045">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2045">Core</span></span>

* <span data-ttu-id="44718-2046">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="44718-2046">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="44718-2047">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-2047">ACR</span></span>

* <span data-ttu-id="44718-2048">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="44718-2048">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="44718-2049">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-2049">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="44718-2050">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="44718-2050">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2051">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2051">ACS</span></span>

* <span data-ttu-id="44718-2052">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2052">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="44718-2053">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2053">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2054">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2054">Appservice</span></span>

* <span data-ttu-id="44718-2055">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="44718-2055">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="44718-2056">Komponente</span><span class="sxs-lookup"><span data-stu-id="44718-2056">Component</span></span>

* <span data-ttu-id="44718-2057">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2057">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-2058">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-2058">Monitor</span></span>

* <span data-ttu-id="44718-2059">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2059">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2060">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2060">Resource</span></span>

* <span data-ttu-id="44718-2061">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2061">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="44718-2062">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="44718-2062">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2063">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2063">VM</span></span>

* <span data-ttu-id="44718-2064">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2064">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="44718-2065">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2065">October 9, 2017</span></span>

<span data-ttu-id="44718-2066">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="44718-2066">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="44718-2067">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2067">Core</span></span>

* <span data-ttu-id="44718-2068">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-2068">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2069">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2069">Appservice</span></span>

* <span data-ttu-id="44718-2070">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-2070">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="44718-2071">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-2071">Batch</span></span>

* <span data-ttu-id="44718-2072">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="44718-2072">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="44718-2073">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="44718-2073">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="44718-2074">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2074">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="44718-2075">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2075">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="44718-2076">BatchAI</span><span class="sxs-lookup"><span data-stu-id="44718-2076">Batchai</span></span>

* <span data-ttu-id="44718-2077">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-2077">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-2078">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-2078">Keyvault</span></span>

* <span data-ttu-id="44718-2079">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="44718-2079">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="44718-2080">(#4448)</span><span class="sxs-lookup"><span data-stu-id="44718-2080">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="44718-2081">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2081">Network</span></span>

* <span data-ttu-id="44718-2082">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="44718-2082">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="44718-2083">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="44718-2083">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2084">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2084">Resource</span></span>

* <span data-ttu-id="44718-2085">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2085">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="44718-2086">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-2086">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="44718-2087">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-2087">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="44718-2088">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-2088">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2089">Sql</span><span class="sxs-lookup"><span data-stu-id="44718-2089">Sql</span></span>

* <span data-ttu-id="44718-2090">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2090">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="44718-2091">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-2091">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="44718-2092">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="44718-2092">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2093">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2093">Storage</span></span>

* <span data-ttu-id="44718-2094">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2094">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2095">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2095">Vm</span></span>

* <span data-ttu-id="44718-2096">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="44718-2096">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="44718-2097">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2097">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="44718-2098">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2098">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="44718-2099">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2099">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="44718-2100">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2100">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="44718-2101">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2101">September 22, 2017</span></span>

<span data-ttu-id="44718-2102">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="44718-2102">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2103">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2103">Resource</span></span>

* <span data-ttu-id="44718-2104">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2104">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="44718-2105">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2105">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="44718-2106">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2106">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="44718-2107">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="44718-2107">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="44718-2108">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2108">Network</span></span>

* <span data-ttu-id="44718-2109">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2109">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="44718-2110">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2110">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="44718-2111">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2111">Added `asg` application security group commands</span></span>
* <span data-ttu-id="44718-2112">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2112">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="44718-2113">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2113">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="44718-2114">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2114">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="44718-2115">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2115">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2116">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2116">Storage</span></span>

* <span data-ttu-id="44718-2117">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="44718-2117">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="44718-2118">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="44718-2118">Eventgrid</span></span>

* <span data-ttu-id="44718-2119">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-2119">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2120">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-2120">SQL</span></span>

* <span data-ttu-id="44718-2121">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="44718-2121">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="44718-2122">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44718-2122">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="44718-2123">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2123">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-2124">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-2124">Keyvault</span></span>

* <span data-ttu-id="44718-2125">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2125">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2126">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2126">VM</span></span>

* <span data-ttu-id="44718-2127">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2127">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="44718-2128">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="44718-2128">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="44718-2129">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2129">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="44718-2130">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2130">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="44718-2131">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2131">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="44718-2132">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2132">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2133">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2133">ACS</span></span>

* <span data-ttu-id="44718-2134">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2134">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2135">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2135">Appservice</span></span>

* <span data-ttu-id="44718-2136">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="44718-2136">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="44718-2137">Backup</span><span class="sxs-lookup"><span data-stu-id="44718-2137">Backup</span></span>

* <span data-ttu-id="44718-2138">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="44718-2138">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="44718-2139">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2139">September 11, 2017</span></span>

<span data-ttu-id="44718-2140">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="44718-2140">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="44718-2141">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2141">Core</span></span>

* <span data-ttu-id="44718-2142">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="44718-2142">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="44718-2143">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="44718-2143">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2144">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2144">Acs</span></span>

* <span data-ttu-id="44718-2145">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2145">Added `acs list-locations` command</span></span>
* <span data-ttu-id="44718-2146">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="44718-2146">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2147">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2147">Appservice</span></span>

* <span data-ttu-id="44718-2148">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="44718-2148">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-2149">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-2149">CDN</span></span>

* <span data-ttu-id="44718-2150">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="44718-2150">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="44718-2151">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="44718-2151">Extension</span></span>

* <span data-ttu-id="44718-2152">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-2152">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-2153">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-2153">Keyvault</span></span>

* <span data-ttu-id="44718-2154">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="44718-2154">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="44718-2155">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2155">Network</span></span>

* <span data-ttu-id="44718-2156">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2156">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="44718-2157">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="44718-2157">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="44718-2158">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2158">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="44718-2159">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2159">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="44718-2160">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2160">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2161">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2161">Resource</span></span>

* <span data-ttu-id="44718-2162">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="44718-2162">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="44718-2163">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="44718-2163">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="44718-2164">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="44718-2164">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="44718-2165">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="44718-2165">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2166">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-2166">SQL</span></span>

* <span data-ttu-id="44718-2167">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2167">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2168">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2168">VM</span></span>

* <span data-ttu-id="44718-2169">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="44718-2169">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="44718-2170">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="44718-2170">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="44718-2171">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2171">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="44718-2172">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="44718-2172">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="44718-2173">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="44718-2173">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="44718-2174">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2174">August 31, 2017</span></span>

<span data-ttu-id="44718-2175">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="44718-2175">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-2176">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-2176">Keyvault</span></span>

* <span data-ttu-id="44718-2177">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="44718-2177">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="44718-2178">Sf</span><span class="sxs-lookup"><span data-stu-id="44718-2178">Sf</span></span>

* <span data-ttu-id="44718-2179">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="44718-2179">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2180">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2180">Storage</span></span>

* <span data-ttu-id="44718-2181">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="44718-2181">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="44718-2182">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="44718-2182">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="44718-2183">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2183">August 28, 2017</span></span>

<span data-ttu-id="44718-2184">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="44718-2184">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="44718-2185">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="44718-2185">CLI</span></span>

* <span data-ttu-id="44718-2186">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2186">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2187">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2187">ACS</span></span>

* <span data-ttu-id="44718-2188">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-2188">Corrected preview regions</span></span>
* <span data-ttu-id="44718-2189">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="44718-2189">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="44718-2190">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="44718-2190">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2191">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2191">Appservice</span></span>

* <span data-ttu-id="44718-2192">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2192">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="44718-2193">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2193">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="44718-2194">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-2194">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="44718-2195">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="44718-2195">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="44718-2196">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="44718-2196">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="44718-2197">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-2197">IoT</span></span>

* <span data-ttu-id="44718-2198">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="44718-2198">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="44718-2199">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2199">Network</span></span>

* <span data-ttu-id="44718-2200">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2200">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="44718-2201">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2201">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="44718-2202">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2202">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="44718-2203">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2203">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="44718-2204">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2204">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-2205">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-2205">Profile</span></span>

* <span data-ttu-id="44718-2206">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-2206">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="44718-2207">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="44718-2207">Service Fabric</span></span>

* <span data-ttu-id="44718-2208">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="44718-2208">Preview release</span></span>
* <span data-ttu-id="44718-2209">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="44718-2209">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="44718-2210">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2210">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="44718-2211">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2211">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2212">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2212">Storage</span></span>

* <span data-ttu-id="44718-2213">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-2213">Enabled setting blob tier</span></span>
* <span data-ttu-id="44718-2214">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2214">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="44718-2215">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2215">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="44718-2216">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-2216">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="44718-2217">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2217">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="44718-2218">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="44718-2218">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2219">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2219">VM</span></span>

* <span data-ttu-id="44718-2220">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2220">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="44718-2221">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-2221">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="44718-2222">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2222">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="44718-2223">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-2223">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="44718-2224">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2224">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="44718-2225">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-2225">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="44718-2226">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2226">August 15, 2017</span></span>

<span data-ttu-id="44718-2227">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="44718-2227">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2228">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2228">ACS</span></span>

* <span data-ttu-id="44718-2229">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-2229">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2230">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2230">Appservice</span></span>

* <span data-ttu-id="44718-2231">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2231">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="44718-2232">Event Grid</span><span class="sxs-lookup"><span data-stu-id="44718-2232">Event Grid</span></span>

* <span data-ttu-id="44718-2233">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2233">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="44718-2234">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2234">August 11, 2017</span></span>

<span data-ttu-id="44718-2235">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="44718-2235">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2236">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2236">ACS</span></span>

* <span data-ttu-id="44718-2237">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2237">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="44718-2238">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-2238">Batch</span></span>

* <span data-ttu-id="44718-2239">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-2239">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="44718-2240">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2240">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="44718-2241">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2241">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="44718-2242">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="44718-2242">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="44718-2243">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="44718-2243">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="44718-2244">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2244">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="44718-2245">Komponente</span><span class="sxs-lookup"><span data-stu-id="44718-2245">Component</span></span>

* <span data-ttu-id="44718-2246">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2246">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="44718-2247">Container</span><span class="sxs-lookup"><span data-stu-id="44718-2247">Container</span></span>

* <span data-ttu-id="44718-2248">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="44718-2248">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="44718-2249">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="44718-2249">Data Lake Store</span></span>

* <span data-ttu-id="44718-2250">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-2250">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="44718-2251">Event Grid</span><span class="sxs-lookup"><span data-stu-id="44718-2251">Event Grid</span></span>

* <span data-ttu-id="44718-2252">Erste Version</span><span class="sxs-lookup"><span data-stu-id="44718-2252">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="44718-2253">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2253">Network</span></span>

* <span data-ttu-id="44718-2254">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2254">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="44718-2255">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="44718-2255">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="44718-2256">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-2256">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="44718-2257">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="44718-2257">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="44718-2258">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-2258">Profile</span></span>

* <span data-ttu-id="44718-2259">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="44718-2259">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2260">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2260">Storage</span></span>

* <span data-ttu-id="44718-2261">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-2261">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2262">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2262">VM</span></span>

* <span data-ttu-id="44718-2263">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-2263">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="44718-2264">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-2264">Exposed `list-skus` command</span></span>
* <span data-ttu-id="44718-2265">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="44718-2265">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="44718-2266">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="44718-2266">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="44718-2267">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2267">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="44718-2268">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2268">July 28, 2017</span></span>

<span data-ttu-id="44718-2269">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="44718-2269">Version 2.0.12</span></span>

* <span data-ttu-id="44718-2270">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2270">Added container commands</span></span>
* <span data-ttu-id="44718-2271">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2271">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="44718-2272">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2272">Core</span></span>

* <span data-ttu-id="44718-2273">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="44718-2273">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="44718-2274">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2274">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="44718-2275">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="44718-2275">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="44718-2276">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="44718-2276">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="44718-2277">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="44718-2277">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="44718-2278">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="44718-2278">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="44718-2279">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="44718-2279">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="44718-2280">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="44718-2280">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="44718-2281">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="44718-2281">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="44718-2282">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="44718-2282">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="44718-2283">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="44718-2283">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="44718-2284">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="44718-2284">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="44718-2285">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="44718-2285">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="44718-2286">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="44718-2286">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="44718-2287">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="44718-2287">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="44718-2288">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="44718-2288">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="44718-2289">ACR</span><span class="sxs-lookup"><span data-stu-id="44718-2289">ACR</span></span>

* <span data-ttu-id="44718-2290">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2290">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="44718-2291">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="44718-2291">Support SKU update for managed registries</span></span>
* <span data-ttu-id="44718-2292">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2292">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="44718-2293">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2293">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="44718-2294">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2294">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="44718-2295">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2295">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2296">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2296">ACS</span></span>

* <span data-ttu-id="44718-2297">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="44718-2297">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2298">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2298">Appservice</span></span>

* <span data-ttu-id="44718-2299">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="44718-2299">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="44718-2300">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="44718-2300">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="44718-2301">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="44718-2301">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="44718-2302">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="44718-2302">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="44718-2303">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="44718-2303">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="44718-2304">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="44718-2304">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="44718-2305">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="44718-2305">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="44718-2306">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="44718-2306">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="44718-2307">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="44718-2307">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="44718-2308">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="44718-2308">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="44718-2309">Batch</span><span class="sxs-lookup"><span data-stu-id="44718-2309">Batch</span></span>

* <span data-ttu-id="44718-2310">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-2310">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="44718-2311">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2311">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="44718-2312">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2312">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="44718-2313">CDN</span><span class="sxs-lookup"><span data-stu-id="44718-2313">CDN</span></span>

* <span data-ttu-id="44718-2314">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="44718-2314">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="44718-2315">Cloud</span><span class="sxs-lookup"><span data-stu-id="44718-2315">Cloud</span></span>

* <span data-ttu-id="44718-2316">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="44718-2316">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="44718-2317">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="44718-2317">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="44718-2318">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="44718-2318">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="44718-2319">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="44718-2319">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="44718-2320">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="44718-2320">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-2321">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-2321">CosmosDB</span></span>

* <span data-ttu-id="44718-2322">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="44718-2322">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="44718-2323">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2323">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="44718-2324">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="44718-2324">Data Lake Analytics</span></span>

* <span data-ttu-id="44718-2325">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2325">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="44718-2326">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2326">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="44718-2327">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2327">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="44718-2328">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="44718-2328">Data Lake Store</span></span>

* <span data-ttu-id="44718-2329">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2329">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="44718-2330">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="44718-2330">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="44718-2331">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="44718-2331">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="44718-2332">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="44718-2332">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="44718-2333">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="44718-2333">Interactive</span></span>

* <span data-ttu-id="44718-2334">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-2334">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="44718-2335">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-2335">Increased test coverage</span></span>
* <span data-ttu-id="44718-2336">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="44718-2336">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="44718-2337">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="44718-2337">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="44718-2338">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="44718-2338">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="44718-2339">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="44718-2339">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="44718-2340">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="44718-2340">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="44718-2341">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2341">Added `--progress` flag</span></span>
* <span data-ttu-id="44718-2342">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2342">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="44718-2343">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="44718-2343">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="44718-2344">IoT</span><span class="sxs-lookup"><span data-stu-id="44718-2344">IoT</span></span>

* <span data-ttu-id="44718-2345">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="44718-2345">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="44718-2346">(3934)</span><span class="sxs-lookup"><span data-stu-id="44718-2346">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="44718-2347">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="44718-2347">Key vault</span></span>

* <span data-ttu-id="44718-2348">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="44718-2348">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="44718-2349">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="44718-2349">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="44718-2350">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="44718-2350">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="44718-2351">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="44718-2351">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="44718-2352">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="44718-2352">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="44718-2353">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="44718-2353">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="44718-2354">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="44718-2354">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="44718-2355">(3307)</span><span class="sxs-lookup"><span data-stu-id="44718-2355">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="44718-2356">Labor</span><span class="sxs-lookup"><span data-stu-id="44718-2356">Lab</span></span>

* <span data-ttu-id="44718-2357">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2357">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="44718-2358">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2358">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-2359">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-2359">Monitor</span></span>

* <span data-ttu-id="44718-2360">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="44718-2360">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="44718-2361">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2361">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="44718-2362">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2362">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="44718-2363">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2363">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="44718-2364">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="44718-2364">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="44718-2365">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="44718-2365">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="44718-2366">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="44718-2366">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="44718-2367">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="44718-2367">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="44718-2368">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="44718-2368">`location` no longer required</span></span>
  * <span data-ttu-id="44718-2369">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="44718-2369">Add name and ID support for target</span></span>
  * <span data-ttu-id="44718-2370">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="44718-2370">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="44718-2371">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="44718-2371">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="44718-2372">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="44718-2372">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="44718-2373">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="44718-2373">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="44718-2374">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="44718-2374">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="44718-2375">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2375">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="44718-2376">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2376">Network</span></span>

* <span data-ttu-id="44718-2377">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2377">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="44718-2378">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2378">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="44718-2379">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="44718-2379">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="44718-2380">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="44718-2380">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="44718-2381">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="44718-2381">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="44718-2382">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2382">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="44718-2383">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="44718-2383">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="44718-2384">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="44718-2384">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="44718-2385">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="44718-2385">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="44718-2386">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="44718-2386">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="44718-2387">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2387">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="44718-2388">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2388">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="44718-2389">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="44718-2389">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="44718-2390">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2390">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="44718-2391">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2391">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="44718-2392">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2392">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="44718-2393">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="44718-2393">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="44718-2394">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="44718-2394">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="44718-2395">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2395">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="44718-2396">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-2396">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="44718-2397">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="44718-2397">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="44718-2398">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="44718-2398">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="44718-2399">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-2399">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="44718-2400">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="44718-2400">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="44718-2401">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="44718-2401">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="44718-2402">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="44718-2402">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="44718-2403">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="44718-2403">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="44718-2404">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-2404">Profile</span></span>

* <span data-ttu-id="44718-2405">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="44718-2405">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="44718-2406">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="44718-2406">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="44718-2407">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="44718-2407">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="44718-2408">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2408">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="44718-2409">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="44718-2409">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="44718-2410">RDBMS</span><span class="sxs-lookup"><span data-stu-id="44718-2410">RDBMS</span></span>

* <span data-ttu-id="44718-2411">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="44718-2411">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="44718-2412">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="44718-2412">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="44718-2413">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="44718-2413">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="44718-2414">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="44718-2414">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2415">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2415">Resource</span></span>

* <span data-ttu-id="44718-2416">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-2416">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="44718-2417">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="44718-2417">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="44718-2418">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2418">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="44718-2419">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="44718-2419">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="44718-2420">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="44718-2420">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="44718-2421">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="44718-2421">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="44718-2422">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="44718-2422">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="44718-2423">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2423">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="44718-2424">Role</span><span class="sxs-lookup"><span data-stu-id="44718-2424">Role</span></span>

* <span data-ttu-id="44718-2425">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="44718-2425">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="44718-2426">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="44718-2426">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="44718-2427">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="44718-2427">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="44718-2428">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="44718-2428">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="44718-2429">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2429">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="44718-2430">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="44718-2430">Service Fabric</span></span>
* <span data-ttu-id="44718-2431">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="44718-2431">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="44718-2432">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="44718-2432">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="44718-2433">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="44718-2433">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2434">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-2434">SQL</span></span>

* <span data-ttu-id="44718-2435">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2435">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="44718-2436">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="44718-2436">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="44718-2437">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2437">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2438">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2438">Storage</span></span>

* <span data-ttu-id="44718-2439">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="44718-2439">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="44718-2440">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="44718-2440">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="44718-2441">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="44718-2441">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="44718-2442">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="44718-2442">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="44718-2443">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="44718-2443">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="44718-2444">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="44718-2444">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2445">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2445">VM</span></span>

* <span data-ttu-id="44718-2446">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="44718-2446">Support configuring nsg</span></span>
* <span data-ttu-id="44718-2447">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="44718-2447">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="44718-2448">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="44718-2448">Support managed service identities</span></span>
* <span data-ttu-id="44718-2449">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="44718-2449">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="44718-2450">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="44718-2450">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="44718-2451">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2451">May 10, 2017</span></span>

<span data-ttu-id="44718-2452">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="44718-2452">Version 2.0.6</span></span>

* <span data-ttu-id="44718-2453">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="44718-2453">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="44718-2454">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="44718-2454">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="44718-2455">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="44718-2455">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="44718-2456">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-2456">Include Cognitive Services module</span></span>
* <span data-ttu-id="44718-2457">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-2457">Include Service Fabric module</span></span>
* <span data-ttu-id="44718-2458">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="44718-2458">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="44718-2459">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="44718-2459">Add support for CDN commands</span></span>
* <span data-ttu-id="44718-2460">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="44718-2460">Remove Container module</span></span>
* <span data-ttu-id="44718-2461">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="44718-2461">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="44718-2462">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="44718-2462">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="44718-2463">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2463">Core</span></span>

* <span data-ttu-id="44718-2464">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="44718-2464">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="44718-2465">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="44718-2465">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="44718-2466">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="44718-2466">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="44718-2467">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="44718-2467">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="44718-2468">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="44718-2468">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="44718-2469">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="44718-2469">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="44718-2470">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="44718-2470">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="44718-2471">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="44718-2471">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="44718-2472">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="44718-2472">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="44718-2473">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="44718-2473">core: Improved performance</span></span>
* <span data-ttu-id="44718-2474">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="44718-2474">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="44718-2475">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="44718-2475">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2476">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2476">ACS</span></span>

* <span data-ttu-id="44718-2477">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44718-2477">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="44718-2478">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="44718-2478">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="44718-2479">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="44718-2479">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="44718-2480">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="44718-2480">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2481">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2481">AppService</span></span>

* <span data-ttu-id="44718-2482">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="44718-2482">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="44718-2483">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="44718-2483">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="44718-2484">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="44718-2484">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="44718-2485">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="44718-2485">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="44718-2486">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="44718-2486">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="44718-2487">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="44718-2487">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="44718-2488">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="44718-2488">support slot swap with preview</span></span>
* <span data-ttu-id="44718-2489">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="44718-2489">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="44718-2490">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="44718-2490">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="44718-2491">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="44718-2491">CosmosDB</span></span>

* <span data-ttu-id="44718-2492">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="44718-2492">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="44718-2493">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="44718-2493">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="44718-2494">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="44718-2494">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="44718-2495">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="44718-2495">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="44718-2496">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="44718-2496">Data Lake Analytics</span></span>

* <span data-ttu-id="44718-2497">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="44718-2497">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="44718-2498">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="44718-2498">Add support for new catalog item type: package.</span></span> <span data-ttu-id="44718-2499">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="44718-2499">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="44718-2500">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="44718-2500">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="44718-2501">Table</span><span class="sxs-lookup"><span data-stu-id="44718-2501">Table</span></span>
  * <span data-ttu-id="44718-2502">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="44718-2502">Table valued function</span></span>
  * <span data-ttu-id="44718-2503">Sicht</span><span class="sxs-lookup"><span data-stu-id="44718-2503">View</span></span>
  * <span data-ttu-id="44718-2504">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="44718-2504">Table Statistics.</span></span> <span data-ttu-id="44718-2505">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="44718-2505">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="44718-2506">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="44718-2506">Data Lake Store</span></span>

* <span data-ttu-id="44718-2507">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="44718-2507">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="44718-2508">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="44718-2508">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="44718-2509">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="44718-2509">missed help for access show.</span></span> <span data-ttu-id="44718-2510">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="44718-2510">adding it.</span></span> <span data-ttu-id="44718-2511">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="44718-2511">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="44718-2512">Suchen</span><span class="sxs-lookup"><span data-stu-id="44718-2512">Find</span></span>

* <span data-ttu-id="44718-2513">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="44718-2513">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="44718-2514">KeyVault</span><span class="sxs-lookup"><span data-stu-id="44718-2514">KeyVault</span></span>

* <span data-ttu-id="44718-2515">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="44718-2515">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="44718-2516">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="44718-2516">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="44718-2517">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="44718-2517">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="44718-2518">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="44718-2518">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="44718-2519">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="44718-2519">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="44718-2520">Labor</span><span class="sxs-lookup"><span data-stu-id="44718-2520">Lab</span></span>

* <span data-ttu-id="44718-2521">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="44718-2521">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="44718-2522">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="44718-2522">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="44718-2523">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="44718-2523">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="44718-2524">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="44718-2524">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="44718-2525">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="44718-2525">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="44718-2526">Überwachen</span><span class="sxs-lookup"><span data-stu-id="44718-2526">Monitor</span></span>

* <span data-ttu-id="44718-2527">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="44718-2527">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="44718-2528">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="44718-2528">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="44718-2529">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2529">Network</span></span>

* <span data-ttu-id="44718-2530">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="44718-2530">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="44718-2531">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="44718-2531">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="44718-2532">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="44718-2532">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="44718-2533">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="44718-2533">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="44718-2534">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="44718-2534">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="44718-2535">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="44718-2535">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="44718-2536">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="44718-2536">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="44718-2537">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="44718-2537">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="44718-2538">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="44718-2538">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="44718-2539">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="44718-2539">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="44718-2540">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="44718-2540">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="44718-2541">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="44718-2541">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="44718-2542">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="44718-2542">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="44718-2543">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="44718-2543">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="44718-2544">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="44718-2544">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="44718-2545">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="44718-2545">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="44718-2546">Profil</span><span class="sxs-lookup"><span data-stu-id="44718-2546">Profile</span></span>

* <span data-ttu-id="44718-2547">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="44718-2547">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="44718-2548">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="44718-2548">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="44718-2549">Redis</span><span class="sxs-lookup"><span data-stu-id="44718-2549">Redis</span></span>

* <span data-ttu-id="44718-2550">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="44718-2550">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="44718-2551">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="44718-2551">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="44718-2552">Resource</span><span class="sxs-lookup"><span data-stu-id="44718-2552">Resource</span></span>

* <span data-ttu-id="44718-2553">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="44718-2553">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="44718-2554">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="44718-2554">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="44718-2555">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="44718-2555">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="44718-2556">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="44718-2556">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="44718-2557">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="44718-2557">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="44718-2558">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="44718-2558">Add docs for az lock update.</span></span> <span data-ttu-id="44718-2559">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="44718-2559">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="44718-2560">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="44718-2560">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="44718-2561">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="44718-2561">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="44718-2562">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="44718-2562">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="44718-2563">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="44718-2563">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="44718-2564">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="44718-2564">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="44718-2565">Role</span><span class="sxs-lookup"><span data-stu-id="44718-2565">Role</span></span>

* <span data-ttu-id="44718-2566">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="44718-2566">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="44718-2567">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="44718-2567">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="44718-2568">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="44718-2568">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="44718-2569">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="44718-2569">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="44718-2570">SQL</span><span class="sxs-lookup"><span data-stu-id="44718-2570">SQL</span></span>

* <span data-ttu-id="44718-2571">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="44718-2571">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="44718-2572">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="44718-2572">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="44718-2573">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2573">Storage</span></span>

* <span data-ttu-id="44718-2574">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="44718-2574">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="44718-2575">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="44718-2575">Add support for incremental blob copy</span></span>
* <span data-ttu-id="44718-2576">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="44718-2576">Add support for large block blob upload</span></span>
* <span data-ttu-id="44718-2577">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="44718-2577">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2578">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2578">VM</span></span>

* <span data-ttu-id="44718-2579">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="44718-2579">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="44718-2580">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="44718-2580">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="44718-2581">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="44718-2581">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="44718-2582">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="44718-2582">az vm/vmss disk</span></span>
  3. <span data-ttu-id="44718-2583">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="44718-2583">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="44718-2584">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="44718-2584">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="44718-2585">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="44718-2585">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="44718-2586">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2586">April 3, 2017</span></span>

<span data-ttu-id="44718-2587">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="44718-2587">Version 2.0.2</span></span>

<span data-ttu-id="44718-2588">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="44718-2588">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="44718-2589">Core</span><span class="sxs-lookup"><span data-stu-id="44718-2589">Core</span></span>

* <span data-ttu-id="44718-2590">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="44718-2590">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="44718-2591">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="44718-2591">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="44718-2592">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="44718-2592">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="44718-2593">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="44718-2593">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="44718-2594">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="44718-2594">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="44718-2595">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="44718-2595">Add prompting for missing template parameters.</span></span> <span data-ttu-id="44718-2596">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="44718-2596">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="44718-2597">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="44718-2597">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="44718-2598">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="44718-2598">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="44718-2599">ACS</span><span class="sxs-lookup"><span data-stu-id="44718-2599">ACS</span></span>

* <span data-ttu-id="44718-2600">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="44718-2600">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="44718-2601">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="44718-2601">Add support for ssh key password prompting.</span></span> <span data-ttu-id="44718-2602">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="44718-2602">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="44718-2603">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="44718-2603">Add support for windows clusters.</span></span> <span data-ttu-id="44718-2604">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="44718-2604">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="44718-2605">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="44718-2605">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="44718-2606">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="44718-2606">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="44718-2607">AppService</span><span class="sxs-lookup"><span data-stu-id="44718-2607">AppService</span></span>

* <span data-ttu-id="44718-2608">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="44718-2608">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="44718-2609">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="44718-2609">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="44718-2610">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="44718-2610">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="44718-2611">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="44718-2611">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="44718-2612">DataLake</span><span class="sxs-lookup"><span data-stu-id="44718-2612">DataLake</span></span>

* <span data-ttu-id="44718-2613">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-2613">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="44718-2614">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="44718-2614">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="44718-2615">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="44718-2615">DocuemntDB</span></span>

* <span data-ttu-id="44718-2616">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="44718-2616">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="44718-2617">VM</span><span class="sxs-lookup"><span data-stu-id="44718-2617">VM</span></span>

* <span data-ttu-id="44718-2618">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="44718-2618">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="44718-2619">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="44718-2619">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="44718-2620">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="44718-2620">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="44718-2621">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="44718-2621">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="44718-2622">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="44718-2622">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="44718-2623">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="44718-2623">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="44718-2624">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="44718-2624">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="44718-2625">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="44718-2625">February 27, 2017</span></span>

<span data-ttu-id="44718-2626">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="44718-2626">Version 2.0.0</span></span>

<span data-ttu-id="44718-2627">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="44718-2627">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="44718-2628">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="44718-2628">Container Service (acs)</span></span>
- <span data-ttu-id="44718-2629">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="44718-2629">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="44718-2630">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="44718-2630">Networking</span></span>
- <span data-ttu-id="44718-2631">Storage</span><span class="sxs-lookup"><span data-stu-id="44718-2631">Storage</span></span>

<span data-ttu-id="44718-2632">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="44718-2632">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="44718-2633">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="44718-2633">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="44718-2634">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="44718-2634">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="44718-2635">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="44718-2635">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="44718-2636">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="44718-2636">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="44718-2637">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="44718-2637">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="44718-2638">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="44718-2638">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="44718-2639">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="44718-2639">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="44718-2640">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="44718-2640">Provide feedback from the command line with the `az feedback` command</span></span>


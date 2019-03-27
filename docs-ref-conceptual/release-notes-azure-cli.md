---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4337f2203841d6247e4b487d245138424c63e448
ms.sourcegitcommit: 71c0ccd475524cf4d6db45bba8139fef3262d764
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "58175132"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="0151d-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="0151d-103">Azure CLI release notes</span></span>
## <a name="march-12-2019"></a><span data-ttu-id="0151d-104">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-104">March 12, 2019</span></span>

<span data-ttu-id="0151d-105">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="0151d-105">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="0151d-106">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-106">Core</span></span>

* <span data-ttu-id="0151d-107">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-107">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-108">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-108">ACR</span></span>

* <span data-ttu-id="0151d-109">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-109">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-110">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-110">ACS</span></span>

* <span data-ttu-id="0151d-111">Geändert, sodass das Argument `--listen-address` für `aks browse` ignoriert wird, wenn es von `kubectl` nicht unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-111">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-112">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-112">AppService</span></span>

* <span data-ttu-id="0151d-113">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="0151d-113">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="0151d-114">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-114">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="0151d-115">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="0151d-115">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="0151d-116">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="0151d-116">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="0151d-117">Botservice</span><span class="sxs-lookup"><span data-stu-id="0151d-117">Botservice</span></span>

* <span data-ttu-id="0151d-118">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-118">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0151d-119">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-119">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0151d-120">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-120">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="0151d-121">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="0151d-121">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="0151d-122">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-122">Container</span></span>

* <span data-ttu-id="0151d-123">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-123">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="0151d-124">EventHub</span><span class="sxs-lookup"><span data-stu-id="0151d-124">EventHub</span></span>

* <span data-ttu-id="0151d-125">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-125">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="0151d-126">Suchen</span><span class="sxs-lookup"><span data-stu-id="0151d-126">Find</span></span>

* <span data-ttu-id="0151d-127">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="0151d-127">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0151d-128">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0151d-128">HDInsight</span></span>

* <span data-ttu-id="0151d-129">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-129">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="0151d-130">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-130">Network</span></span>

* <span data-ttu-id="0151d-131">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="0151d-131">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-132">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0151d-132">Rdbms</span></span>

* <span data-ttu-id="0151d-133">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="0151d-133">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="0151d-134">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-134">Role</span></span>

* <span data-ttu-id="0151d-135">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="0151d-135">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="0151d-136">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0151d-136">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0151d-137">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0151d-137">Service Fabric</span></span>

* <span data-ttu-id="0151d-138">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-138">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="0151d-139">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-139">February 26, 2019</span></span>

<span data-ttu-id="0151d-140">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="0151d-140">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="0151d-141">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-141">Core</span></span>

* <span data-ttu-id="0151d-142">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="0151d-142">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-143">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-143">ACR</span></span>

* <span data-ttu-id="0151d-144">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-144">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="0151d-145">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="0151d-145">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-146">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-146">ACS</span></span>

* <span data-ttu-id="0151d-147">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-147">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-148">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-148">AppService</span></span>

* <span data-ttu-id="0151d-149">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-149">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-150">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-150">Batch</span></span>
* <span data-ttu-id="0151d-151">[WICHTIGE ÄNDERUNG] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-151">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="0151d-152">[WICHTIGE ÄNDERUNG] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-152">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="0151d-153">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-153">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="0151d-154">[WICHTIGE ÄNDERUNG] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-154">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="0151d-155">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-155">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="0151d-156">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="0151d-156">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-157">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-157">CosmosDB</span></span>

* <span data-ttu-id="0151d-158">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-158">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="0151d-159">Kusto</span><span class="sxs-lookup"><span data-stu-id="0151d-159">Kusto</span></span>

* <span data-ttu-id="0151d-160">[WICHTIGE ÄNDERUNG] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-160">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="0151d-161">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-161">Network</span></span>

* <span data-ttu-id="0151d-162">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-162">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="0151d-163">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-163">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="0151d-164">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-164">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="0151d-165">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-165">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="0151d-166">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-166">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="0151d-167">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-167">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="0151d-168">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-168">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-169">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-169">Resource</span></span>

* <span data-ttu-id="0151d-170">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-170">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="0151d-171">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-171">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="0151d-172">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-172">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="0151d-173">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-173">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="0151d-174">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-174">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="0151d-175">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-175">Role</span></span>

* <span data-ttu-id="0151d-176">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-176">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-177">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-177">VM</span></span>

* <span data-ttu-id="0151d-178">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="0151d-178">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="0151d-179">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-179">February 12, 2019</span></span>

<span data-ttu-id="0151d-180">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="0151d-180">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="0151d-181">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-181">Core</span></span>

* <span data-ttu-id="0151d-182">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-182">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="0151d-183">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-183">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-184">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-184">ACR</span></span>
* <span data-ttu-id="0151d-185">[WICHTIGE ÄNDERUNG] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-185">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="0151d-186">[WICHTIGE ÄNDERUNG] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-186">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-187">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-187">ACS</span></span>
* <span data-ttu-id="0151d-188">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-188">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="0151d-189">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-189">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="0151d-190">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-190">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="0151d-191">AMS</span><span class="sxs-lookup"><span data-stu-id="0151d-191">AMS</span></span>
* <span data-ttu-id="0151d-192">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-192">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="0151d-193">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-193">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-194">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-194">Appservice</span></span>
* <span data-ttu-id="0151d-195">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-195">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="0151d-196">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-196">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="0151d-197">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0151d-197">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="0151d-198">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-198">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="0151d-199">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-199">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="0151d-200">Botservice</span><span class="sxs-lookup"><span data-stu-id="0151d-200">Botservice</span></span>
* <span data-ttu-id="0151d-201">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0151d-201">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="0151d-202">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-202">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="0151d-203">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-203">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="0151d-204">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="0151d-204">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="0151d-205">[VERALTET] Das `--proj-name`-Argument wurde zugunsten von `--proj-file-path` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-205">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="0151d-206">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="0151d-206">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="0151d-207">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-207">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="0151d-208">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-208">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="0151d-209">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="0151d-209">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="0151d-210">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="0151d-210">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="0151d-211">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0151d-211">Key Vault</span></span>
* <span data-ttu-id="0151d-212">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="0151d-212">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-213">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-213">Monitor</span></span>
* <span data-ttu-id="0151d-214">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-214">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-215">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-215">Network</span></span>
* <span data-ttu-id="0151d-216">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="0151d-216">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="0151d-217">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0151d-217">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="0151d-218">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0151d-218">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="0151d-219">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-219">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0151d-220">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0151d-220">Policy Insights</span></span>
* <span data-ttu-id="0151d-221">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0151d-221">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-222">RDBMS</span></span>
* <span data-ttu-id="0151d-223">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="0151d-223">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="0151d-224">Redis</span><span class="sxs-lookup"><span data-stu-id="0151d-224">Redis</span></span>
* <span data-ttu-id="0151d-225">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-225">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="0151d-226">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-226">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="0151d-227">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-227">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="0151d-228">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-228">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="0151d-229">[WICHTIGE ÄNDERUNG] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-229">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="0151d-230">[WICHTIGE ÄNDERUNG] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-230">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="0151d-231">[VERALTET] Warnmeldung für die Deaktivierung von des Befehls `redis import-method` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-231">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="0151d-232">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-232">Role</span></span>
* <span data-ttu-id="0151d-233">[WICHTIGE ÄNDERUNG] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-233">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="0151d-234">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="0151d-234">SQL VM</span></span>
* <span data-ttu-id="0151d-235">[VERALTET] Das `--boostrap-acc-pwd`-Argument wurde aufgrund eines Tippfehlers als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-235">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-236">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-236">VM</span></span>
* <span data-ttu-id="0151d-237">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="0151d-237">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="0151d-238">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-238">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="0151d-239">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="0151d-239">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="0151d-240">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-240">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="0151d-241">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-241">January 31, 2019</span></span>

<span data-ttu-id="0151d-242">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="0151d-242">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="0151d-243">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-243">Core</span></span>

* <span data-ttu-id="0151d-244">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="0151d-244">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="0151d-245">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-245">January 28, 2019</span></span>

<span data-ttu-id="0151d-246">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="0151d-246">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-247">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-247">ACR</span></span>
* <span data-ttu-id="0151d-248">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-248">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-249">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-249">ACS</span></span>
* <span data-ttu-id="0151d-250">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-250">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0151d-251">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-251">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="0151d-252">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-252">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="0151d-253">AMS</span><span class="sxs-lookup"><span data-stu-id="0151d-253">AMS</span></span>
* <span data-ttu-id="0151d-254">[WICHTIGE ÄNDERUNG] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-254">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="0151d-255">[WICHTIGE ÄNDERUNG] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-255">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-256">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-256">Appservice</span></span>
* <span data-ttu-id="0151d-257">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-257">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="0151d-258">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-258">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="0151d-259">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-259">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="0151d-260">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-260">Container</span></span>
* <span data-ttu-id="0151d-261">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-261">Added `container start` command</span></span>
* <span data-ttu-id="0151d-262">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="0151d-262">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0151d-263">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0151d-263">EventGrid</span></span>
* <span data-ttu-id="0151d-264">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-264">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="0151d-265">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-265">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="0151d-266">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-266">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="0151d-267">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-267">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="0151d-268">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-268">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0151d-269">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0151d-269">HDInsight</span></span>
* <span data-ttu-id="0151d-270">[WICHTIGE ÄNDERUNG] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-270">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="0151d-271">[WICHTIGE ÄNDERUNG] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-271">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="0151d-272">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-272">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="0151d-273">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-273">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="0151d-274">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-274">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="0151d-275">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-275">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-276">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-276">IoT</span></span>
* <span data-ttu-id="0151d-277">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-277">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="0151d-278">Kusto</span><span class="sxs-lookup"><span data-stu-id="0151d-278">Kusto</span></span>
* <span data-ttu-id="0151d-279">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0151d-279">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-280">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-280">Monitor</span></span>
* <span data-ttu-id="0151d-281">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-281">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-282">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-282">Profile</span></span>
* <span data-ttu-id="0151d-283">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0151d-283">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-284">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-284">Network</span></span>
* <span data-ttu-id="0151d-285">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="0151d-285">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="0151d-286">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="0151d-286">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-287">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-287">Resource</span></span>
* <span data-ttu-id="0151d-288">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-288">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="0151d-289">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-289">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="0151d-290">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="0151d-290">SQL Virtual Machine</span></span>
* <span data-ttu-id="0151d-291">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0151d-291">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-292">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-292">Storage</span></span>
* <span data-ttu-id="0151d-293">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-293">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="0151d-294">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-294">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-295">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-295">VM</span></span>
* <span data-ttu-id="0151d-296">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-296">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="0151d-297">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-297">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="0151d-298">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0151d-298">January 15, 2019</span></span>

<span data-ttu-id="0151d-299">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="0151d-299">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-300">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-300">ACR</span></span>
* <span data-ttu-id="0151d-301">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-301">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="0151d-302">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-302">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="0151d-303">[VERALTET] Parameter `--resource-group` wurde in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="0151d-303">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="0151d-304">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-304">ACS</span></span>
* <span data-ttu-id="0151d-305">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-305">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-306">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-306">Appservice</span></span>
* <span data-ttu-id="0151d-307">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="0151d-307">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="0151d-308">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-308">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="0151d-309">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-309">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="0151d-310">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-310">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="0151d-311">Botservice</span><span class="sxs-lookup"><span data-stu-id="0151d-311">Botservice</span></span>
* <span data-ttu-id="0151d-312">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-312">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="0151d-313">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0151d-313">Configure</span></span>
* <span data-ttu-id="0151d-314">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-314">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-315">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-315">CosmosDB</span></span>
* <span data-ttu-id="0151d-316">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-316">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0151d-317">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0151d-317">HDInsight</span></span>
* <span data-ttu-id="0151d-318">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-318">Added commands for managing applications</span></span>
* <span data-ttu-id="0151d-319">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-319">Added commands for managing script actions</span></span>
* <span data-ttu-id="0151d-320">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-320">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="0151d-321">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-321">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="0151d-322">[WICHTIGE ÄNDERUNG] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-322">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-323">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-323">Network</span></span>
* <span data-ttu-id="0151d-324">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-324">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="0151d-325">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="0151d-325">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="0151d-326">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-326">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="0151d-327">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="0151d-327">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="0151d-328">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-328">Role</span></span>
* <span data-ttu-id="0151d-329">[VERALTET] Das `--password`-Argument wurde für `create-for-rbac` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-329">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="0151d-330">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="0151d-330">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="0151d-331">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0151d-331">Security</span></span>
* <span data-ttu-id="0151d-332">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-332">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-333">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-333">Storage</span></span>
* <span data-ttu-id="0151d-334">[WICHTIGE ÄNDERUNG] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="0151d-334">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="0151d-335">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-335">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="0151d-336">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-336">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="0151d-337">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-337">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="0151d-338">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-338">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-339">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-339">VM</span></span>
* <span data-ttu-id="0151d-340">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="0151d-340">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="0151d-341">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-341">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0151d-342">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-342">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="0151d-343">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0151d-343">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="0151d-344">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="0151d-344">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="0151d-345">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="0151d-345">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="0151d-346">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-346">December 20, 2018</span></span>

<span data-ttu-id="0151d-347">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="0151d-347">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="0151d-348">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-348">Appservice</span></span>
* <span data-ttu-id="0151d-349">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-349">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="0151d-350">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-350">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="0151d-351">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-351">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0151d-352">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="0151d-352">IoTCentral</span></span>
* <span data-ttu-id="0151d-353">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-353">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="0151d-354">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-354">Role</span></span>
* <span data-ttu-id="0151d-355">[WICHTIGE ÄNDERUNG] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="0151d-355">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-356">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-356">SQL</span></span>
* <span data-ttu-id="0151d-357">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-357">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-358">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-358">VM</span></span>
* <span data-ttu-id="0151d-359">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-359">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="0151d-360">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-360">December 18, 2018</span></span>

<span data-ttu-id="0151d-361">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="0151d-361">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="0151d-362">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-362">ACR</span></span>
* <span data-ttu-id="0151d-363">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-363">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="0151d-364">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="0151d-364">Condensed the table layout for task list</span></span>
* <span data-ttu-id="0151d-365">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-365">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-366">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-366">ACS</span></span>
* <span data-ttu-id="0151d-367">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-367">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0151d-368">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-368">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="0151d-369">[VERALTET] `az acs`-Befehle als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="0151d-369">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="0151d-370">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="0151d-370">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="0151d-371">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-371">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="0151d-372">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-372">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-373">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-373">Appservice</span></span>
* <span data-ttu-id="0151d-374">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-374">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="0151d-375">Botservice</span><span class="sxs-lookup"><span data-stu-id="0151d-375">Botservice</span></span>
* <span data-ttu-id="0151d-376">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-376">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="0151d-377">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-377">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="0151d-378">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-378">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="0151d-379">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="0151d-379">Reduced Kudu network calls</span></span>
* <span data-ttu-id="0151d-380">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="0151d-380">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-381">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-381">Consumption</span></span>
* <span data-ttu-id="0151d-382">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-382">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-383">CosmosDB</span></span>
* <span data-ttu-id="0151d-384">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-384">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="0151d-385">Karten</span><span class="sxs-lookup"><span data-stu-id="0151d-385">Maps</span></span>
* <span data-ttu-id="0151d-386">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-386">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-387">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-387">Network</span></span>
* <span data-ttu-id="0151d-388">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-388">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="0151d-389">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0151d-389">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-390">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-390">Resource</span></span>
* <span data-ttu-id="0151d-391">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-391">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="0151d-392">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-392">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-393">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-393">Storage</span></span>
*  <span data-ttu-id="0151d-394">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-394">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-395">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-395">VM</span></span>
* <span data-ttu-id="0151d-396">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="0151d-396">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="0151d-397">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-397">December 4, 2018</span></span>

<span data-ttu-id="0151d-398">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="0151d-398">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="0151d-399">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-399">Core</span></span>
* <span data-ttu-id="0151d-400">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-400">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="0151d-401">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-401">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-402">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-402">Appservice</span></span>
* <span data-ttu-id="0151d-403">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="0151d-403">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="0151d-404">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="0151d-404">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="0151d-405">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-405">Network</span></span>
* <span data-ttu-id="0151d-406">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-406">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="0151d-407">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-407">Role</span></span>
* <span data-ttu-id="0151d-408">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-408">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="0151d-409">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-409">VM</span></span>
* <span data-ttu-id="0151d-410">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-410">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="0151d-411">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="0151d-411">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="0151d-412">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0151d-412">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="0151d-413">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="0151d-413">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="0151d-414">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-414">November 20, 2018</span></span>

<span data-ttu-id="0151d-415">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="0151d-415">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="0151d-416">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-416">Core</span></span>
* <span data-ttu-id="0151d-417">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-417">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-418">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-418">ACR</span></span>
* <span data-ttu-id="0151d-419">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-419">Added context token to task step</span></span>
* <span data-ttu-id="0151d-420">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-420">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="0151d-421">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-421">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-422">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-422">Appservice</span></span>
* <span data-ttu-id="0151d-423">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-423">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="0151d-424">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="0151d-424">Updated the default `node_version`.</span></span> <span data-ttu-id="0151d-425">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="0151d-425">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="0151d-426">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-426">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="0151d-427">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="0151d-427">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0151d-428">IotCentral</span><span class="sxs-lookup"><span data-stu-id="0151d-428">IotCentral</span></span>
* <span data-ttu-id="0151d-429">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-429">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-430">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-430">KeyVault</span></span>
* <span data-ttu-id="0151d-431">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-431">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="0151d-432">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-432">Network</span></span>
* <span data-ttu-id="0151d-433">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-433">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="0151d-434">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-434">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="0151d-435">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-435">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="0151d-436">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-436">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-437">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0151d-437">Rdbms</span></span>
* <span data-ttu-id="0151d-438">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-438">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="0151d-439">RBAC</span><span class="sxs-lookup"><span data-stu-id="0151d-439">Rbac</span></span>
* <span data-ttu-id="0151d-440">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-440">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="0151d-441">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-441">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="0151d-442">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-442">Storage</span></span>
* <span data-ttu-id="0151d-443">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-443">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="0151d-444">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="0151d-444">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="0151d-445">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-445">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="0151d-446">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-446">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-447">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-447">VM</span></span>
* <span data-ttu-id="0151d-448">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-448">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="0151d-449">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-449">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="0151d-450">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0151d-450">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="0151d-451">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-451">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="0151d-452">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-452">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="0151d-453">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-453">Added `snapshot wait` command</span></span>
* <span data-ttu-id="0151d-454">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-454">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="0151d-455">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-455">November 6, 2018</span></span>

<span data-ttu-id="0151d-456">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="0151d-456">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="0151d-457">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-457">Core</span></span>
* <span data-ttu-id="0151d-458">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-458">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-459">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-459">ACR</span></span>
* <span data-ttu-id="0151d-460">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-460">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="0151d-461">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-461">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-462">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-462">ACS</span></span>
* <span data-ttu-id="0151d-463">[WICHTIGE ÄNDERUNG] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="0151d-463">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="0151d-464">Advisor</span><span class="sxs-lookup"><span data-stu-id="0151d-464">Advisor</span></span>
* <span data-ttu-id="0151d-465">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="0151d-465">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="0151d-466">AMS</span><span class="sxs-lookup"><span data-stu-id="0151d-466">AMS</span></span>
* <span data-ttu-id="0151d-467">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-467">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="0151d-468">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-468">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="0151d-469">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-469">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="0151d-470">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-470">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="0151d-471">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-471">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="0151d-472">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-472">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="0151d-473">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-473">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="0151d-474">[WICHTIGE ÄNDERUNG] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0151d-474">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="0151d-475">[WICHTIGE ÄNDERUNG] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-475">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="0151d-476">[WICHTIGE ÄNDERUNG] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-476">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="0151d-477">[WICHTIGE ÄNDERUNG] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0151d-477">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="0151d-478">[WICHTIGE ÄNDERUNG] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0151d-478">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="0151d-479">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="0151d-479">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="0151d-480">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-480">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="0151d-481">[WICHTIGE ÄNDERUNG] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0151d-481">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="0151d-482">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-482">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="0151d-483">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="0151d-483">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-484">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-484">AppService</span></span>
* <span data-ttu-id="0151d-485">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="0151d-485">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="0151d-486">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0151d-486">Configure</span></span>
* <span data-ttu-id="0151d-487">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-487">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="0151d-488">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-488">Container</span></span>
* <span data-ttu-id="0151d-489">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="0151d-489">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="0151d-490">EventHub</span><span class="sxs-lookup"><span data-stu-id="0151d-490">EventHub</span></span>
* <span data-ttu-id="0151d-491">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-491">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-492">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-492">Interactive</span></span>
* <span data-ttu-id="0151d-493">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-493">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-494">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-494">Monitor</span></span>
* <span data-ttu-id="0151d-495">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-495">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-496">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-496">Network</span></span>
* <span data-ttu-id="0151d-497">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-497">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="0151d-498">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="0151d-498">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="0151d-499">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="0151d-499">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="0151d-500">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-500">Profile</span></span>
* <span data-ttu-id="0151d-501">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-501">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-502">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-502">RDBMS</span></span>
* <span data-ttu-id="0151d-503">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-503">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-504">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-504">Resource</span></span>
* <span data-ttu-id="0151d-505">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-505">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="0151d-506">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-506">Role</span></span>
* <span data-ttu-id="0151d-507">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-507">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="0151d-508">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="0151d-508">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="0151d-509">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-509">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-510">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-510">Storage</span></span>
* <span data-ttu-id="0151d-511">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="0151d-511">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-512">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-512">VM</span></span>
* <span data-ttu-id="0151d-513">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-513">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="0151d-514">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="0151d-514">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="0151d-515">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-515">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="0151d-516">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="0151d-516">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="0151d-517">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-517">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="0151d-518">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-518">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="0151d-519">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-519">October 23, 2018</span></span>

<span data-ttu-id="0151d-520">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="0151d-520">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="0151d-521">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-521">Core</span></span>
* <span data-ttu-id="0151d-522">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="0151d-522">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="0151d-523">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="0151d-523">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-524">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-524">ACR</span></span>
* <span data-ttu-id="0151d-525">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-525">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="0151d-526">CDN</span><span class="sxs-lookup"><span data-stu-id="0151d-526">CDN</span></span>
* <span data-ttu-id="0151d-527">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-527">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0151d-528">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0151d-528">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="0151d-529">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-529">Container</span></span>
* <span data-ttu-id="0151d-530">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-530">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="0151d-531">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="0151d-531">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="0151d-532">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-532">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="0151d-533">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="0151d-533">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="0151d-534">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0151d-534">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="0151d-535">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-535">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="0151d-536">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-536">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-537">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-537">CosmosDB</span></span>
* <span data-ttu-id="0151d-538">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-538">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-539">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-539">Interactive</span></span>
* <span data-ttu-id="0151d-540">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-540">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="0151d-541">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0151d-541">IoT Central</span></span>
* <span data-ttu-id="0151d-542">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-542">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="0151d-543">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0151d-543">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-544">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-544">Monitor</span></span>
* <span data-ttu-id="0151d-545">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="0151d-545">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="0151d-546">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-546">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="0151d-547">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0151d-548">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="0151d-549">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-549">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="0151d-550">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-550">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="0151d-551">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="0151d-551">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="0151d-552">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-552">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0151d-553">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-553">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="0151d-554">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-554">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-555">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-555">Network</span></span>
* <span data-ttu-id="0151d-556">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-556">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="0151d-557">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-557">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="0151d-558">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0151d-558">ServiceBus</span></span>
* <span data-ttu-id="0151d-559">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-559">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-560">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-560">SQL</span></span>
* <span data-ttu-id="0151d-561">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="0151d-561">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-562">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-562">Storage</span></span>
* <span data-ttu-id="0151d-563">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-563">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="0151d-564">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-564">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-565">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-565">VM</span></span>
* <span data-ttu-id="0151d-566">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="0151d-566">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="0151d-567">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-567">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="0151d-568">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-568">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="0151d-569">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-569">October 16, 2018</span></span>

<span data-ttu-id="0151d-570">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="0151d-570">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-571">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-571">VM</span></span>
* <span data-ttu-id="0151d-572">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="0151d-572">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="0151d-573">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-573">October 9, 2018</span></span>

<span data-ttu-id="0151d-574">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="0151d-574">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="0151d-575">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-575">Core</span></span>
* <span data-ttu-id="0151d-576">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="0151d-576">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-577">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-577">ACR</span></span>
* <span data-ttu-id="0151d-578">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-578">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-579">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-579">ACS</span></span>
* <span data-ttu-id="0151d-580">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="0151d-580">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="0151d-581">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="0151d-581">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="0151d-582">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="0151d-582">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="0151d-583">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="0151d-583">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="0151d-584">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-584">Container</span></span>
* <span data-ttu-id="0151d-585">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-585">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="0151d-586">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-586">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="0151d-587">Event Hub</span><span class="sxs-lookup"><span data-stu-id="0151d-587">Event Hub</span></span>
* <span data-ttu-id="0151d-588">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-588">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="0151d-589">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-589">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="0151d-590">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0151d-590">Extensions</span></span>
* <span data-ttu-id="0151d-591">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="0151d-591">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0151d-592">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0151d-592">HDInsight</span></span>
* <span data-ttu-id="0151d-593">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-593">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-594">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-594">IoT</span></span>
* <span data-ttu-id="0151d-595">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-595">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-596">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-596">KeyVault</span></span>
* <span data-ttu-id="0151d-597">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="0151d-597">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="0151d-598">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-598">Network</span></span>
* <span data-ttu-id="0151d-599">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="0151d-599">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="0151d-600">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="0151d-600">See #6052</span></span>
* <span data-ttu-id="0151d-601">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="0151d-601">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="0151d-602">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="0151d-602">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="0151d-603">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-603">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="0151d-604">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-604">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="0151d-605">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0151d-605">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="0151d-606">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-606">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="0151d-607">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-607">Role</span></span>
* <span data-ttu-id="0151d-608">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-608">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="0151d-609">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-609">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="0151d-610">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0151d-610">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="0151d-611">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="0151d-611">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="0151d-612">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0151d-612">Service Bus</span></span>
* <span data-ttu-id="0151d-613">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-613">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-614">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-614">VM</span></span>
* <span data-ttu-id="0151d-615">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-615">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="0151d-616">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="0151d-616">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="0151d-617">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-617">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="0151d-618">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-618">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="0151d-619">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-619">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="0151d-620">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-620">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="0151d-621">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-621">September 21, 2018</span></span>

<span data-ttu-id="0151d-622">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="0151d-622">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-623">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-623">ACR</span></span>
* <span data-ttu-id="0151d-624">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-624">Added ACR Task commands</span></span>
* <span data-ttu-id="0151d-625">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-625">Added quick run command</span></span>
* <span data-ttu-id="0151d-626">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-626">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="0151d-627">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-627">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="0151d-628">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-628">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="0151d-629">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-629">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-630">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-630">ACS</span></span>
* <span data-ttu-id="0151d-631">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-631">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="0151d-632">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-632">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-633">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-633">AppService</span></span>

* <span data-ttu-id="0151d-634">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="0151d-634">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="0151d-635">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-635">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="0151d-636">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-636">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="0151d-637">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-637">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-638">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-638">Batch</span></span>
* <span data-ttu-id="0151d-639">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-639">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="0151d-640">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-640">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="0151d-641">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-641">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="0151d-642">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-642">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0151d-643">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-643">Batch AI</span></span> 
* <span data-ttu-id="0151d-644">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-644">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0151d-645">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0151d-645">Cognitive Services</span></span>
* <span data-ttu-id="0151d-646">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-646">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="0151d-647">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-647">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="0151d-648">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-648">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="0151d-649">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-649">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="0151d-650">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-650">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="0151d-651">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="0151d-651">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="0151d-652">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-652">Container</span></span>
* <span data-ttu-id="0151d-653">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-653">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="0151d-654">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-654">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="0151d-655">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-655">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="0151d-656">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-656">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="0151d-657">Data Lake</span><span class="sxs-lookup"><span data-stu-id="0151d-657">Datalake</span></span>
* <span data-ttu-id="0151d-658">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-658">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="0151d-659">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="0151d-659">Interactive Shell</span></span>
* <span data-ttu-id="0151d-660">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-660">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="0151d-661">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-661">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-662">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-662">IoT</span></span>
* <span data-ttu-id="0151d-663">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-663">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="0151d-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0151d-664">Key Vault</span></span>
* <span data-ttu-id="0151d-665">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-665">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="0151d-666">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-666">Network</span></span>
* <span data-ttu-id="0151d-667">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-667">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="0151d-668">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-668">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="0151d-669">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-669">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="0151d-670">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-670">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="0151d-671">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-671">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="0151d-672">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-672">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="0151d-673">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-673">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="0151d-674">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="0151d-674">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="0151d-675">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-675">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="0151d-676">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-676">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="0151d-677">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-677">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="0151d-678">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-678">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="0151d-679">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-679">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="0151d-680">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="0151d-680">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="0151d-681">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-681">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="0151d-682">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="0151d-682">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="0151d-683">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-683">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="0151d-684">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-684">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-685">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-685">RDBMS</span></span>
* <span data-ttu-id="0151d-686">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-686">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="0151d-687">Reservierung</span><span class="sxs-lookup"><span data-stu-id="0151d-687">Reservation</span></span>
* <span data-ttu-id="0151d-688">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-688">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="0151d-689">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-689">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="0151d-690">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="0151d-690">Manage App</span></span>
* <span data-ttu-id="0151d-691">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="0151d-691">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="0151d-692">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="0151d-692">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="0151d-693">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-693">Role</span></span>
* <span data-ttu-id="0151d-694">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-694">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="0151d-695">SignalR</span><span class="sxs-lookup"><span data-stu-id="0151d-695">SignalR</span></span>
* <span data-ttu-id="0151d-696">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-696">First release</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-697">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-697">Storage</span></span>
* <span data-ttu-id="0151d-698">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-698">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="0151d-699">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-699">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-700">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-700">VM</span></span>
* <span data-ttu-id="0151d-701">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="0151d-701">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="0151d-702">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-702">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="0151d-703">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-703">August 28, 2018</span></span>

<span data-ttu-id="0151d-704">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="0151d-704">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="0151d-705">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-705">Core</span></span>

* <span data-ttu-id="0151d-706">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-706">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="0151d-707">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-707">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-708">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-708">ACR</span></span>

* <span data-ttu-id="0151d-709">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-709">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="0151d-710">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="0151d-710">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-711">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-711">ACS</span></span>

* <span data-ttu-id="0151d-712">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-712">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="0151d-713">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="0151d-713">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-714">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-714">AppService</span></span>

* <span data-ttu-id="0151d-715">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-715">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="0151d-716">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-716">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="0151d-717">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-717">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="0151d-718">Backup</span><span class="sxs-lookup"><span data-stu-id="0151d-718">Backup</span></span>

* <span data-ttu-id="0151d-719">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-719">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="0151d-720">Botdienst</span><span class="sxs-lookup"><span data-stu-id="0151d-720">Bot Service</span></span>

* <span data-ttu-id="0151d-721">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="0151d-721">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0151d-722">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0151d-722">Cognitive Services</span></span>

* <span data-ttu-id="0151d-723">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="0151d-723">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-724">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-724">IoT</span></span>

* <span data-ttu-id="0151d-725">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-725">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-726">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-726">Monitor</span></span>

* <span data-ttu-id="0151d-727">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-727">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="0151d-728">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-728">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0151d-729">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-729">Network</span></span>

* <span data-ttu-id="0151d-730">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-730">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-731">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-731">Resource</span></span>

* <span data-ttu-id="0151d-732">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-732">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-733">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-733">Storage</span></span>

* <span data-ttu-id="0151d-734">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-734">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-735">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-735">VM</span></span>

* <span data-ttu-id="0151d-736">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0151d-736">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="0151d-737">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="0151d-737">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="0151d-738">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-738">Auguest 14, 2018</span></span>

<span data-ttu-id="0151d-739">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="0151d-739">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="0151d-740">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-740">Core</span></span>

* <span data-ttu-id="0151d-741">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-741">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="0151d-742">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-742">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="0151d-743">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="0151d-743">Telemetry</span></span>

* <span data-ttu-id="0151d-744">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="0151d-744">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-745">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-745">ACR</span></span>

* <span data-ttu-id="0151d-746">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-746">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="0151d-747">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-747">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-748">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-748">ACS</span></span>

* <span data-ttu-id="0151d-749">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-749">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="0151d-750">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0151d-750">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="0151d-751">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="0151d-751">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="0151d-752">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="0151d-752">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="0151d-753">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0151d-753">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="0151d-754">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-754">AppService</span></span>

* <span data-ttu-id="0151d-755">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="0151d-755">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="0151d-756">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-756">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="0151d-757">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-757">BatchAI</span></span>

* <span data-ttu-id="0151d-758">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0151d-758">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="0151d-759">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-759">Container</span></span>

* <span data-ttu-id="0151d-760">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-760">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="0151d-761">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-761">IoT</span></span>

* <span data-ttu-id="0151d-762">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-762">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="0151d-763">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="0151d-763">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="0151d-764">Iot Central</span><span class="sxs-lookup"><span data-stu-id="0151d-764">Iot Central</span></span>

* <span data-ttu-id="0151d-765">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-765">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-766">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-766">KeyVault</span></span>


* <span data-ttu-id="0151d-767">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-767">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="0151d-768">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-768">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="0151d-769">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-769">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="0151d-770">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-770">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="0151d-771">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-771">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="0151d-772">Relay</span><span class="sxs-lookup"><span data-stu-id="0151d-772">Relay</span></span>

* <span data-ttu-id="0151d-773">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-773">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-774">Sql</span><span class="sxs-lookup"><span data-stu-id="0151d-774">Sql</span></span>

* <span data-ttu-id="0151d-775">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-775">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-776">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-776">Storage</span></span>

* <span data-ttu-id="0151d-777">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="0151d-777">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="0151d-778">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="0151d-778">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="0151d-779">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-779">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="0151d-780">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="0151d-780">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="0151d-781">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="0151d-781">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-782">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-782">VM</span></span>

* <span data-ttu-id="0151d-783">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-783">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="0151d-784">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-784">July 31, 2018</span></span>

<span data-ttu-id="0151d-785">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="0151d-785">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-786">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-786">ACR</span></span>

* <span data-ttu-id="0151d-787">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-787">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="0151d-788">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-788">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-789">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-789">ACS</span></span>

* <span data-ttu-id="0151d-790">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-790">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-791">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-791">Batch</span></span>

* <span data-ttu-id="0151d-792">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0151d-792">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="0151d-793">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-793">Container</span></span>

* <span data-ttu-id="0151d-794">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-794">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="0151d-795">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-795">Network</span></span>

* <span data-ttu-id="0151d-796">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-796">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="0151d-797">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-797">Resource</span></span>

* <span data-ttu-id="0151d-798">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="0151d-798">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="0151d-799">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="0151d-799">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="0151d-800">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-800">Role</span></span>

* <span data-ttu-id="0151d-801">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-801">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="0151d-802">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0151d-802">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="0151d-803">Suchen,</span><span class="sxs-lookup"><span data-stu-id="0151d-803">Search</span></span>

* <span data-ttu-id="0151d-804">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-804">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="0151d-805">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0151d-805">Service Bus</span></span>

* <span data-ttu-id="0151d-806">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="0151d-806">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="0151d-807">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-807">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="0151d-808">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="0151d-808">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="0151d-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="0151d-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-810">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-810">Storage</span></span>

* <span data-ttu-id="0151d-811">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-811">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="0151d-812">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-812">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-813">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-813">VM</span></span>

* <span data-ttu-id="0151d-814">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-814">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="0151d-815">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-815">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="0151d-816">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-816">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="0151d-817">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-817">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="0151d-818">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-818">July 18, 2018</span></span>

<span data-ttu-id="0151d-819">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="0151d-819">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="0151d-820">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-820">Core</span></span>

* <span data-ttu-id="0151d-821">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-821">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="0151d-822">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-822">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="0151d-823">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="0151d-823">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-824">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-824">ACR</span></span>

* <span data-ttu-id="0151d-825">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-825">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="0151d-826">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-826">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="0151d-827">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-827">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="0151d-828">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-828">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-829">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-829">ACS</span></span>

* <span data-ttu-id="0151d-830">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="0151d-830">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-831">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-831">AppService</span></span>

* <span data-ttu-id="0151d-832">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-832">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-833">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-833">Batch</span></span>

* <span data-ttu-id="0151d-834">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="0151d-834">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="0151d-835">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-835">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0151d-836">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-836">Batch AI</span></span>

* <span data-ttu-id="0151d-837">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-837">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="0151d-838">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-838">Container</span></span>

* <span data-ttu-id="0151d-839">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-839">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="0151d-840">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-840">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="0151d-841">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-841">Network</span></span>

* <span data-ttu-id="0151d-842">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-842">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="0151d-843">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-843">Added `network nic wait`</span></span>
* <span data-ttu-id="0151d-844">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-844">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="0151d-845">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="0151d-845">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="0151d-846">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-846">Resource</span></span>

* <span data-ttu-id="0151d-847">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-847">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="0151d-848">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-848">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="0151d-849">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-849">Added `deployment wait` command</span></span>
* <span data-ttu-id="0151d-850">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-850">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-851">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-851">SQL</span></span>

* <span data-ttu-id="0151d-852">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-852">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="0151d-853">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="0151d-853">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="0151d-854">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-854">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-855">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-855">Storage</span></span>

* <span data-ttu-id="0151d-856">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-856">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-857">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-857">VM</span></span>

* <span data-ttu-id="0151d-858">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-858">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="0151d-859">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-859">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="0151d-860">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-860">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0151d-861">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-861">July 3, 2018</span></span>

<span data-ttu-id="0151d-862">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="0151d-862">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="0151d-863">AKS</span><span class="sxs-lookup"><span data-stu-id="0151d-863">AKS</span></span>

* <span data-ttu-id="0151d-864">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-864">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0151d-865">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-865">July 3, 2018</span></span>

<span data-ttu-id="0151d-866">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="0151d-866">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="0151d-867">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-867">Core</span></span>

* <span data-ttu-id="0151d-868">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-868">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-869">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-869">ACR</span></span>

* <span data-ttu-id="0151d-870">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-870">Added polling build status</span></span>
* <span data-ttu-id="0151d-871">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-871">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="0151d-872">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-872">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-873">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-873">ACS</span></span>

* <span data-ttu-id="0151d-874">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0151d-874">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="0151d-875">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="0151d-875">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="0151d-876">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-876">Updated options for `aks browse` command.</span></span> <span data-ttu-id="0151d-877">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-877">Added `--listen-port` support</span></span>
* <span data-ttu-id="0151d-878">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-878">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="0151d-879">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="0151d-879">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="0151d-880">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-880">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-881">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-881">AppService</span></span>

* <span data-ttu-id="0151d-882">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-882">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="0151d-883">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-883">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="0151d-884">Backup</span><span class="sxs-lookup"><span data-stu-id="0151d-884">Backup</span></span>

* <span data-ttu-id="0151d-885">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-885">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="0151d-886">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-886">BatchAI</span></span>

* <span data-ttu-id="0151d-887">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-887">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="0151d-888">Cloud</span><span class="sxs-lookup"><span data-stu-id="0151d-888">Cloud</span></span>

* <span data-ttu-id="0151d-889">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-889">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="0151d-890">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-890">Container</span></span>

* <span data-ttu-id="0151d-891">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-891">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="0151d-892">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-892">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="0151d-893">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-893">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-894">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-894">Extension</span></span>

* <span data-ttu-id="0151d-895">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-895">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="0151d-896">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-896">Network</span></span>

* <span data-ttu-id="0151d-897">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="0151d-897">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0151d-898">Rdbms</span></span>

* <span data-ttu-id="0151d-899">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-899">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-900">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-900">Resource</span></span>

* <span data-ttu-id="0151d-901">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-901">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-902">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-902">VM</span></span>

* <span data-ttu-id="0151d-903">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-903">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="0151d-904">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-904">June 25, 2018</span></span>

<span data-ttu-id="0151d-905">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="0151d-905">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="0151d-906">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="0151d-906">CLI</span></span>

* <span data-ttu-id="0151d-907">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="0151d-907">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="0151d-908">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-908">June 19, 2018</span></span>

<span data-ttu-id="0151d-909">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="0151d-909">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="0151d-910">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-910">Core</span></span>

* <span data-ttu-id="0151d-911">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-911">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-912">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-912">ACR</span></span>

* <span data-ttu-id="0151d-913">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-913">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="0151d-914">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="0151d-914">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-915">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-915">ACS</span></span>

* <span data-ttu-id="0151d-916">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0151d-916">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="0151d-917">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-917">Added `--update` support</span></span>
* <span data-ttu-id="0151d-918">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-918">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="0151d-919">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-919">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="0151d-920">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-920">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="0151d-921">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="0151d-921">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="0151d-922">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-922">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="0151d-923">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-923">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-924">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-924">AppService</span></span>

* <span data-ttu-id="0151d-925">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-925">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="0151d-926">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-926">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-927">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-927">Batch</span></span>

* <span data-ttu-id="0151d-928">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-928">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0151d-929">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-929">Batch AI</span></span>

* <span data-ttu-id="0151d-930">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-930">Added support for workspaces.</span></span> <span data-ttu-id="0151d-931">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="0151d-931">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="0151d-932">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-932">Added support for experiments.</span></span> <span data-ttu-id="0151d-933">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="0151d-933">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="0151d-934">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-934">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="0151d-935">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-935">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="0151d-936">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="0151d-936">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="0151d-937">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-937">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="0151d-938">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-938">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="0151d-939">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-939">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="0151d-940">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-940">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="0151d-941">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="0151d-941">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="0151d-942">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-942">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="0151d-943">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="0151d-943">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="0151d-944">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-944">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="0151d-945">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="0151d-945">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="0151d-946">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-946">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="0151d-947">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="0151d-947">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="0151d-948">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-948">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="0151d-949">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-949">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0151d-950">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-950">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0151d-951">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-951">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="0151d-952">Karten</span><span class="sxs-lookup"><span data-stu-id="0151d-952">Maps</span></span>

* <span data-ttu-id="0151d-953">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0151d-953">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="0151d-954">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-954">Network</span></span>

* <span data-ttu-id="0151d-955">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="0151d-955">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="0151d-956">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="0151d-956">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="0151d-957">#6502</span><span class="sxs-lookup"><span data-stu-id="0151d-957">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="0151d-958">Reservations</span><span class="sxs-lookup"><span data-stu-id="0151d-958">Reservations</span></span>

* <span data-ttu-id="0151d-959">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-959">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="0151d-960">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-960">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="0151d-961">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-961">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="0151d-962">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-962">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="0151d-963">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-963">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="0151d-964">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-964">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="0151d-965">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-965">Role</span></span>

* <span data-ttu-id="0151d-966">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-966">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-967">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-967">SQL</span></span>

* <span data-ttu-id="0151d-968">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="0151d-968">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-969">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-969">Storage</span></span>

* <span data-ttu-id="0151d-970">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-970">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-971">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-971">VM</span></span>

* <span data-ttu-id="0151d-972">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="0151d-972">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="0151d-973">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-973">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="0151d-974">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-974">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0151d-975">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-975">June 13, 2018</span></span>

<span data-ttu-id="0151d-976">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="0151d-976">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="0151d-977">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-977">Core</span></span>

* <span data-ttu-id="0151d-978">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="0151d-978">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0151d-979">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-979">June 13, 2018</span></span>

<span data-ttu-id="0151d-980">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="0151d-980">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="0151d-981">AKS</span><span class="sxs-lookup"><span data-stu-id="0151d-981">AKS</span></span>

* <span data-ttu-id="0151d-982">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-982">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="0151d-983">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-983">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="0151d-984">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-984">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="0151d-985">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-985">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="0151d-986">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-986">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-987">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-987">AppService</span></span>

* <span data-ttu-id="0151d-988">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-988">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0151d-989">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-989">June 5, 2018</span></span>

<span data-ttu-id="0151d-990">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="0151d-990">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-991">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-991">Interactive</span></span>

* <span data-ttu-id="0151d-992">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-992">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0151d-993">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-993">June 5, 2018</span></span>

<span data-ttu-id="0151d-994">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="0151d-994">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="0151d-995">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-995">Core</span></span>

* <span data-ttu-id="0151d-996">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-996">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="0151d-997">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="0151d-997">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-998">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-998">ACR</span></span>

* <span data-ttu-id="0151d-999">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-999">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="0151d-1000">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1000">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="0151d-1001">AKS</span><span class="sxs-lookup"><span data-stu-id="0151d-1001">AKS</span></span>

* <span data-ttu-id="0151d-1002">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1002">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1003">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1003">Batch</span></span>

* <span data-ttu-id="0151d-1004">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="0151d-1004">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1005">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1005">IOT</span></span>

* <span data-ttu-id="0151d-1006">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1006">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1007">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1007">Network</span></span>

* <span data-ttu-id="0151d-1008">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0151d-1008">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0151d-1009">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0151d-1009">Policy Insights</span></span>

* <span data-ttu-id="0151d-1010">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1010">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="0151d-1011">ARM</span><span class="sxs-lookup"><span data-stu-id="0151d-1011">ARM</span></span>

* <span data-ttu-id="0151d-1012">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1012">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1013">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1013">SQL</span></span>

* <span data-ttu-id="0151d-1014">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1014">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="0151d-1015">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1015">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="0151d-1016">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1016">Storage</span></span>

* <span data-ttu-id="0151d-1017">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="0151d-1017">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1018">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1018">VM</span></span>

* <span data-ttu-id="0151d-1019">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-1019">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="0151d-1020">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1020">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="0151d-1021">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1021">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="0151d-1022">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1022">May 22, 2018</span></span>

<span data-ttu-id="0151d-1023">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="0151d-1023">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1024">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1024">Core</span></span>

* <span data-ttu-id="0151d-1025">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1025">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1026">ACS</span></span>

* <span data-ttu-id="0151d-1027">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1027">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="0151d-1028">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1028">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1029">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1029">AppService</span></span>

* <span data-ttu-id="0151d-1030">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="0151d-1030">Improved generic update commands</span></span>
* <span data-ttu-id="0151d-1031">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1031">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1032">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1032">Container</span></span>

* <span data-ttu-id="0151d-1033">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1033">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="0151d-1034">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1034">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1035">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1035">Extension</span></span>

* <span data-ttu-id="0151d-1036">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0151d-1036">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1037">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1037">Interactive</span></span>

* <span data-ttu-id="0151d-1038">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="0151d-1038">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="0151d-1039">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="0151d-1039">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-1040">KeyVault</span></span>

* <span data-ttu-id="0151d-1041">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0151d-1041">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1042">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1042">Network</span></span>

* <span data-ttu-id="0151d-1043">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="0151d-1043">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="0151d-1044">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="0151d-1044">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1045">SQL</span></span>

* <span data-ttu-id="0151d-1046">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="0151d-1046">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="0151d-1047">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1047">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="0151d-1048">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1048">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="0151d-1049">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="0151d-1049">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="0151d-1050">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1050">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="0151d-1051">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1051">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="0151d-1052">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="0151d-1052">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="0151d-1053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1053">`edition`.</span></span> <span data-ttu-id="0151d-1054">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="0151d-1054">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="0151d-1055">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1055">`elasticPoolName`.</span></span> <span data-ttu-id="0151d-1056">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="0151d-1056">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="0151d-1057">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1057">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="0151d-1058">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1058">`edition`.</span></span> <span data-ttu-id="0151d-1059">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1059">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="0151d-1060">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1060">`dtu`.</span></span> <span data-ttu-id="0151d-1061">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1061">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="0151d-1062">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1062">`databaseDtuMin`.</span></span> <span data-ttu-id="0151d-1063">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1063">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="0151d-1064">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1064">`databaseDtuMax`.</span></span> <span data-ttu-id="0151d-1065">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1065">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="0151d-1066">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1066">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="0151d-1067">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1067">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1068">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1068">Storage</span></span>

* <span data-ttu-id="0151d-1069">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1069">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="0151d-1070">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1070">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1071">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1071">VM</span></span>

* <span data-ttu-id="0151d-1072">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1072">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="0151d-1073">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-1073">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="0151d-1074">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1074">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="0151d-1075">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1075">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="0151d-1076">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1076">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="0151d-1077">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1077">May 7, 2018</span></span>

<span data-ttu-id="0151d-1078">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="0151d-1078">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1079">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1079">Core</span></span>

* <span data-ttu-id="0151d-1080">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="0151d-1080">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="0151d-1081">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1081">Added limited support for positional arguments</span></span>
* <span data-ttu-id="0151d-1082">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-1082">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="0151d-1083">#5591</span><span class="sxs-lookup"><span data-stu-id="0151d-1083">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="0151d-1084">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1084">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="0151d-1085">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="0151d-1085">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="0151d-1086">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="0151d-1086">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="0151d-1087">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="0151d-1087">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="0151d-1088">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1088">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1089">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1089">ACR</span></span>

* <span data-ttu-id="0151d-1090">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1090">Added ACR Build commands</span></span>
* <span data-ttu-id="0151d-1091">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1091">Improved resource not found error messages</span></span>
* <span data-ttu-id="0151d-1092">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="0151d-1092">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="0151d-1093">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1093">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="0151d-1094">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1094">Improved repository commands error messages</span></span>
* <span data-ttu-id="0151d-1095">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1095">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1096">ACS</span></span>

* <span data-ttu-id="0151d-1097">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="0151d-1097">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="0151d-1098">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1098">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="0151d-1099">AMS</span><span class="sxs-lookup"><span data-stu-id="0151d-1099">AMS</span></span>

* <span data-ttu-id="0151d-1100">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="0151d-1100">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1101">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1101">Appservice</span></span>

* <span data-ttu-id="0151d-1102">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="0151d-1102">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="0151d-1103">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1103">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="0151d-1104">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1104">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="0151d-1105">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1105">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0151d-1106">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-1106">Batch AI</span></span>

* <span data-ttu-id="0151d-1107">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1107">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0151d-1108">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0151d-1108">Cognitive Services</span></span>

* <span data-ttu-id="0151d-1109">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="0151d-1109">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-1110">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-1110">Consumption</span></span>

* <span data-ttu-id="0151d-1111">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1111">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1112">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1112">Container</span></span>

* <span data-ttu-id="0151d-1113">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-1113">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0151d-1114">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0151d-1114">Cosmos DB</span></span>

* <span data-ttu-id="0151d-1115">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0151d-1115">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="0151d-1116">DMS</span><span class="sxs-lookup"><span data-stu-id="0151d-1116">DMS</span></span>

* <span data-ttu-id="0151d-1117">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1117">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1118">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1118">Extension</span></span>

* <span data-ttu-id="0151d-1119">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1119">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1120">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1120">Interactive</span></span>

* <span data-ttu-id="0151d-1121">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="0151d-1121">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="0151d-1122">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="0151d-1122">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="0151d-1123">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1123">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="0151d-1124">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1124">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="0151d-1125">Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-1125">Lab</span></span>

* <span data-ttu-id="0151d-1126">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1126">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1127">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1127">Network</span></span>

* <span data-ttu-id="0151d-1128">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="0151d-1128">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="0151d-1129">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1129">Profile</span></span>

* <span data-ttu-id="0151d-1130">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1130">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="0151d-1131">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="0151d-1131">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="0151d-1132">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1132">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="0151d-1133">Redis</span><span class="sxs-lookup"><span data-stu-id="0151d-1133">Redis</span></span>

* <span data-ttu-id="0151d-1134">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1134">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="0151d-1135">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1135">Deprecated `redis list-all`.</span></span> <span data-ttu-id="0151d-1136">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="0151d-1136">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="0151d-1137">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1137">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="0151d-1138">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1138">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="0151d-1139">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1139">Role</span></span>

* <span data-ttu-id="0151d-1140">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1140">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1141">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1141">Storage</span></span>

* <span data-ttu-id="0151d-1142">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="0151d-1142">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="0151d-1143">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="0151d-1143">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="0151d-1144">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="0151d-1144">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="0151d-1145">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="0151d-1145">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="0151d-1146">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0151d-1146">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1147">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1147">VM</span></span>

* <span data-ttu-id="0151d-1148">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1148">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="0151d-1149">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1149">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="0151d-1150">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="0151d-1150">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="0151d-1151">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1151">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="0151d-1152">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="0151d-1152">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="0151d-1153">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1153">Added write accelerator support</span></span>
* <span data-ttu-id="0151d-1154">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1154">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="0151d-1155">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="0151d-1155">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="0151d-1156">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="0151d-1156">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="0151d-1157">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1157">April 10, 2018</span></span>

<span data-ttu-id="0151d-1158">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="0151d-1158">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1159">ACR</span></span>

* <span data-ttu-id="0151d-1160">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="0151d-1160">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1161">ACS</span></span>

* <span data-ttu-id="0151d-1162">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1162">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1163">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1163">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="0151d-1165">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1165">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="0151d-1166">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0151d-1166">BatchAI</span></span>

* <span data-ttu-id="0151d-1167">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1167">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="0151d-1168">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="0151d-1168">Job level mounting</span></span>
  - <span data-ttu-id="0151d-1169">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="0151d-1169">Environment variables with secret values</span></span>
  - <span data-ttu-id="0151d-1170">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="0151d-1170">Performance counters settings</span></span>
  - <span data-ttu-id="0151d-1171">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="0151d-1171">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="0151d-1172">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="0151d-1172">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="0151d-1173">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="0151d-1173">Usage and limits reporting</span></span>
  - <span data-ttu-id="0151d-1174">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="0151d-1174">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="0151d-1175">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="0151d-1175">Support for custom images</span></span>
  - <span data-ttu-id="0151d-1176">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1176">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="0151d-1177">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="0151d-1177">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="0151d-1178">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="0151d-1178">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="0151d-1179">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="0151d-1179">National clouds are supported</span></span>
* <span data-ttu-id="0151d-1180">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1180">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="0151d-1181">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="0151d-1181">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="0151d-1182">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1182">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="0151d-1183">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="0151d-1183">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="0151d-1184">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="0151d-1184">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="0151d-1185">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="0151d-1185">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="0151d-1186">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="0151d-1186">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="0151d-1187">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1187">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="0151d-1188">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="0151d-1188">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="0151d-1189">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1189">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="0151d-1190">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="0151d-1190">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="0151d-1191">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1191">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="0151d-1192">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="0151d-1192">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="0151d-1193">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="0151d-1193">Billing</span></span>

* <span data-ttu-id="0151d-1194">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1194">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-1195">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-1195">Consumption</span></span>

* <span data-ttu-id="0151d-1196">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1196">Added `marketplace` commands</span></span>
* <span data-ttu-id="0151d-1197">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1197">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="0151d-1198">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1198">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="0151d-1199">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1199">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="0151d-1200">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1200">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="0151d-1201">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1201">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1202">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1202">Container</span></span>

* <span data-ttu-id="0151d-1203">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1203">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="0151d-1204">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-1204">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1205">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1205">Extension</span></span>

* <span data-ttu-id="0151d-1206">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1206">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1207">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1207">Interactive</span></span>

* <span data-ttu-id="0151d-1208">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="0151d-1208">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="0151d-1209">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1209">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="0151d-1210">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1210">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1211">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1211">Network</span></span>

* <span data-ttu-id="0151d-1212">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-1212">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="0151d-1213">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1213">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="0151d-1214">#4910</span><span class="sxs-lookup"><span data-stu-id="0151d-1214">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="0151d-1215">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1215">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="0151d-1216">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1216">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="0151d-1217">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1217">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="0151d-1218">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1218">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="0151d-1219">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1219">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1220">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1220">Profile</span></span>

* <span data-ttu-id="0151d-1221">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1221">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="0151d-1222">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1222">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-1223">RDBMS</span></span>

* <span data-ttu-id="0151d-1224">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1224">Added `georestore` command</span></span>
* <span data-ttu-id="0151d-1225">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1225">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1226">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1226">Resource</span></span>

* <span data-ttu-id="0151d-1227">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1227">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="0151d-1228">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1228">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1229">SQL</span></span>

* <span data-ttu-id="0151d-1230">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1230">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1231">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1231">Storage</span></span>

* <span data-ttu-id="0151d-1232">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1232">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1233">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1233">VM</span></span>

* <span data-ttu-id="0151d-1234">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1234">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="0151d-1235">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1235">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="0151d-1237">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1237">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="0151d-1238">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="0151d-1238">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="0151d-1239">#5718</span><span class="sxs-lookup"><span data-stu-id="0151d-1239">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="0151d-1240">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="0151d-1240">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="0151d-1241">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1241">March 27, 2018</span></span>

<span data-ttu-id="0151d-1242">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="0151d-1242">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1243">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1243">Core</span></span>

* <span data-ttu-id="0151d-1244">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="0151d-1244">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1245">ACS</span></span>

* <span data-ttu-id="0151d-1246">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0151d-1246">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1247">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1247">Appservice</span></span>

* <span data-ttu-id="0151d-1248">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1248">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="0151d-1249">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1249">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0151d-1250">Backup</span><span class="sxs-lookup"><span data-stu-id="0151d-1250">Backup</span></span>

* <span data-ttu-id="0151d-1251">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1251">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="0151d-1252">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="0151d-1252">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="0151d-1253">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="0151d-1253">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="0151d-1254">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="0151d-1254">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1255">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1255">Container</span></span>

* <span data-ttu-id="0151d-1256">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1256">Added `container exec` command.</span></span> <span data-ttu-id="0151d-1257">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0151d-1257">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="0151d-1258">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0151d-1258">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1259">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1259">Extension</span></span>

* <span data-ttu-id="0151d-1260">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="0151d-1260">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="0151d-1261">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-1261">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="0151d-1262">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-1262">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1263">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1263">Interactive</span></span>

* <span data-ttu-id="0151d-1264">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-1264">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="0151d-1265">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1265">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="0151d-1266">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0151d-1266">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="0151d-1267">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="0151d-1267">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="0151d-1268">Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-1268">Lab</span></span>

* <span data-ttu-id="0151d-1269">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1269">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1270">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1270">Monitor</span></span>

* <span data-ttu-id="0151d-1271">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="0151d-1271">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="0151d-1272">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="0151d-1272">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="0151d-1273">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="0151d-1273">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1274">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1274">Network</span></span>

* <span data-ttu-id="0151d-1275">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1275">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1276">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1276">Profile</span></span>

* <span data-ttu-id="0151d-1277">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1277">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-1278">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-1278">RDBMS</span></span>

* <span data-ttu-id="0151d-1279">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1279">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1280">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1280">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="0151d-1282">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1282">Role</span></span>

* <span data-ttu-id="0151d-1283">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1283">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="0151d-1284">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0151d-1284">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="0151d-1285">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1285">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="0151d-1286">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1286">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="0151d-1287">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1287">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1288">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1288">Storage</span></span>

* <span data-ttu-id="0151d-1289">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1289">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="0151d-1290">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="0151d-1290">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1291">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1291">VM</span></span>

* <span data-ttu-id="0151d-1292">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1292">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="0151d-1293">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1293">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="0151d-1294">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="0151d-1294">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="0151d-1295">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0151d-1295">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="0151d-1296">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1296">March 13, 2018</span></span>

<span data-ttu-id="0151d-1297">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="0151d-1297">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1298">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1298">ACR</span></span>

* <span data-ttu-id="0151d-1299">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1299">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="0151d-1300">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1300">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="0151d-1301">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1301">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1302">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1302">ACS</span></span>

* <span data-ttu-id="0151d-1303">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1303">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="0151d-1304">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1304">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="0151d-1305">Advisor</span><span class="sxs-lookup"><span data-stu-id="0151d-1305">Advisor</span></span>

* <span data-ttu-id="0151d-1306">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1306">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="0151d-1307">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1307">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="0151d-1308">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1308">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="0151d-1309">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1309">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="0151d-1310">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1310">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1311">Appservice</span></span>

* <span data-ttu-id="0151d-1312">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1312">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="0151d-1313">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1313">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0151d-1314">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0151d-1314">Eventhubs</span></span>

* <span data-ttu-id="0151d-1315">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1315">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1316">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1316">Extension</span></span>

* <span data-ttu-id="0151d-1317">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="0151d-1317">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1318">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1318">Interactive</span></span>

* <span data-ttu-id="0151d-1319">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="0151d-1319">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="0151d-1320">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="0151d-1320">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="0151d-1321">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0151d-1321">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="0151d-1322">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1322">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1323">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1323">Monitor</span></span>

* <span data-ttu-id="0151d-1324">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1324">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="0151d-1325">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1325">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="0151d-1326">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1326">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="0151d-1327">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1327">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1328">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1328">Network</span></span>

* <span data-ttu-id="0151d-1329">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1329">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="0151d-1330">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1330">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="0151d-1331">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1331">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="0151d-1332">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1332">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1333">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1333">Profile</span></span>

* <span data-ttu-id="0151d-1334">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1334">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="0151d-1335">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1335">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-1336">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-1336">RDBMS</span></span>

* <span data-ttu-id="0151d-1337">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1337">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="0151d-1338">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0151d-1338">Service Bus</span></span>

* <span data-ttu-id="0151d-1339">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1339">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1340">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1340">Storage</span></span>

* <span data-ttu-id="0151d-1341">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="0151d-1341">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="0151d-1342">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="0151d-1342">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1343">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1343">VM</span></span>

* <span data-ttu-id="0151d-1344">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="0151d-1344">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="0151d-1345">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1345">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="0151d-1346">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1346">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="0151d-1347">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1347">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="0151d-1348">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1348">February 27, 2018</span></span>

<span data-ttu-id="0151d-1349">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="0151d-1349">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1350">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1350">Core</span></span>

* <span data-ttu-id="0151d-1351">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="0151d-1351">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="0151d-1352">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1352">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="0151d-1353">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1353">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1354">ACS</span></span>

* <span data-ttu-id="0151d-1355">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1355">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="0151d-1356">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0151d-1356">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="0151d-1357">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1357">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="0151d-1358">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1358">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1359">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1359">Appservice</span></span>

* <span data-ttu-id="0151d-1360">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="0151d-1360">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="0151d-1361">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="0151d-1361">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0151d-1362">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0151d-1362">Cognitive Services</span></span>

* <span data-ttu-id="0151d-1363">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1363">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-1364">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-1364">Consumption</span></span>

* <span data-ttu-id="0151d-1365">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1365">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="0151d-1366">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1366">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1367">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1367">Container</span></span>

* <span data-ttu-id="0151d-1368">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="0151d-1368">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1369">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1369">Network</span></span>

* <span data-ttu-id="0151d-1370">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="0151d-1370">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1371">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1371">Resource</span></span>

* <span data-ttu-id="0151d-1372">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="0151d-1372">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="0151d-1373">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1373">Role</span></span>

* <span data-ttu-id="0151d-1374">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1374">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1375">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1375">SQL</span></span>

* <span data-ttu-id="0151d-1376">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="0151d-1376">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1377">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1377">Storage</span></span>

* <span data-ttu-id="0151d-1378">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-1378">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1379">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1379">VM</span></span>

* <span data-ttu-id="0151d-1380">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1380">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="0151d-1381">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1381">February 13, 2018</span></span>

<span data-ttu-id="0151d-1382">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="0151d-1382">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1383">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1383">Core</span></span>

* <span data-ttu-id="0151d-1384">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1384">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1385">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1385">ACS</span></span>

* <span data-ttu-id="0151d-1386">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1386">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="0151d-1387">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1387">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="0151d-1388">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1388">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="0151d-1389">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1389">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="0151d-1390">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1390">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="0151d-1391">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1391">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="0151d-1392">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="0151d-1392">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="0151d-1393">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="0151d-1393">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1394">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1394">Appservice</span></span>

* <span data-ttu-id="0151d-1395">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="0151d-1395">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="0151d-1396">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1396">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="0151d-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="0151d-1397">CDN</span></span>

* <span data-ttu-id="0151d-1398">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1398">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1399">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1399">Container</span></span>

* <span data-ttu-id="0151d-1400">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1400">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="0151d-1401">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1401">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-1402">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-1402">CosmosDB</span></span>

* <span data-ttu-id="0151d-1403">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1403">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1404">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1404">Extension</span></span>

* <span data-ttu-id="0151d-1405">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1405">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="0151d-1406">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1406">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="0151d-1407">Feedback</span><span class="sxs-lookup"><span data-stu-id="0151d-1407">Feedback</span></span>

* <span data-ttu-id="0151d-1408">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1408">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1409">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1409">Interactive</span></span>

* <span data-ttu-id="0151d-1410">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1410">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="0151d-1411">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1411">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1412">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1412">IoT</span></span>

* <span data-ttu-id="0151d-1413">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="0151d-1413">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0151d-1414">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="0151d-1414">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0151d-1415">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1415">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="0151d-1416">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1416">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1417">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1417">Monitor</span></span>

* <span data-ttu-id="0151d-1418">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1418">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1419">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1419">Network</span></span>

* <span data-ttu-id="0151d-1420">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="0151d-1420">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="0151d-1421">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1421">Profile</span></span>

* <span data-ttu-id="0151d-1422">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="0151d-1422">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1423">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1423">Resource</span></span>

* <span data-ttu-id="0151d-1424">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1424">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="0151d-1425">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1425">Role</span></span>

* <span data-ttu-id="0151d-1426">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1426">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1427">SQL</span></span>

* <span data-ttu-id="0151d-1428">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1428">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="0151d-1429">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1429">Added `sql db rename`</span></span>
* <span data-ttu-id="0151d-1430">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1430">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1431">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1431">Storage</span></span>

* <span data-ttu-id="0151d-1432">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1432">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1433">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1433">VM</span></span>

* <span data-ttu-id="0151d-1434">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1434">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="0151d-1435">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1435">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="0151d-1436">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0151d-1436">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="0151d-1437">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1437">January 31, 2018</span></span>

<span data-ttu-id="0151d-1438">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="0151d-1438">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1439">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1439">Core</span></span>

* <span data-ttu-id="0151d-1440">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1440">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="0151d-1441">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1441">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="0151d-1442">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0151d-1442">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="0151d-1443">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="0151d-1443">Use `--verbose` to see</span></span>
* <span data-ttu-id="0151d-1444">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1444">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1445">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1445">ACS</span></span>

* <span data-ttu-id="0151d-1446">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="0151d-1446">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="0151d-1447">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1447">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1448">Appservice</span></span>

* <span data-ttu-id="0151d-1449">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0151d-1449">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="0151d-1450">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1450">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="0151d-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="0151d-1451">CDN</span></span>

* <span data-ttu-id="0151d-1452">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1452">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-1453">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-1453">CosmosDB</span></span>

* <span data-ttu-id="0151d-1454">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1454">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1455">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1455">Interactive</span></span>

* <span data-ttu-id="0151d-1456">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1456">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1457">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1457">Network</span></span>

* <span data-ttu-id="0151d-1458">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1458">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="0151d-1459">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="0151d-1459">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="0151d-1460">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1460">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="0151d-1461">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1461">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="0151d-1462">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1462">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="0151d-1463">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="0151d-1463">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="0151d-1464">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1464">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="0151d-1465">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1465">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="0151d-1466">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1466">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="0151d-1467">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="0151d-1467">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1468">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1468">Profile</span></span>

* <span data-ttu-id="0151d-1469">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1469">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1470">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1470">Resource</span></span>

* <span data-ttu-id="0151d-1471">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="0151d-1471">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1472">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1472">Storage</span></span>

* <span data-ttu-id="0151d-1473">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1473">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="0151d-1474">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1474">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="0151d-1475">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0151d-1475">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="0151d-1476">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1476">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="0151d-1477">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="0151d-1477">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1478">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1478">VM</span></span>

* <span data-ttu-id="0151d-1479">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1479">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="0151d-1480">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="0151d-1480">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="0151d-1481">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1481">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="0151d-1482">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1482">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="0151d-1483">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="0151d-1483">January 17, 2018</span></span>

<span data-ttu-id="0151d-1484">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="0151d-1484">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1485">ACR</span></span>

* <span data-ttu-id="0151d-1486">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1486">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="0151d-1487">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="0151d-1487">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1488">ACS</span></span>

* <span data-ttu-id="0151d-1489">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1489">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="0151d-1490">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1490">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1491">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1491">Appservice</span></span>

* <span data-ttu-id="0151d-1492">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="0151d-1492">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="0151d-1493">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1493">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="0151d-1494">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1494">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="0151d-1495">Backup</span><span class="sxs-lookup"><span data-stu-id="0151d-1495">Backup</span></span>

* <span data-ttu-id="0151d-1496">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="0151d-1496">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="0151d-1497">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1497">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="0151d-1498">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="0151d-1498">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="0151d-1499">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="0151d-1499">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="0151d-1500">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="0151d-1500">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1501">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1501">Batch</span></span>

* <span data-ttu-id="0151d-1502">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0151d-1502">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="0151d-1503">Cloud</span><span class="sxs-lookup"><span data-stu-id="0151d-1503">Cloud</span></span>

* <span data-ttu-id="0151d-1504">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1504">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-1505">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-1505">Consumption</span></span>

* <span data-ttu-id="0151d-1506">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="0151d-1506">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="0151d-1507">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0151d-1507">Event Grid</span></span>

* <span data-ttu-id="0151d-1508">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-1508">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0151d-1509">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-1509">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0151d-1510">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1510">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="0151d-1511">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="0151d-1512">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1512">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="0151d-1513">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1513">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="0151d-1514">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1514">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="0151d-1515">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1515">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1516">Interactive</span><span class="sxs-lookup"><span data-stu-id="0151d-1516">Interactive</span></span>

* <span data-ttu-id="0151d-1517">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-1517">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="0151d-1518">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1518">Fixed errors on startup</span></span>
* <span data-ttu-id="0151d-1519">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="0151d-1519">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1520">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1520">IoT</span></span>

* <span data-ttu-id="0151d-1521">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1521">Added support for device provisioning service</span></span>
* <span data-ttu-id="0151d-1522">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1522">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="0151d-1523">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="0151d-1523">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1524">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1524">Monitor</span></span>

* <span data-ttu-id="0151d-1525">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1525">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="0151d-1526">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0151d-1526">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="0151d-1527">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1527">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1528">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1528">Network</span></span>

* <span data-ttu-id="0151d-1529">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="0151d-1529">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="0151d-1530">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1530">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1531">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1531">Profile</span></span>

* <span data-ttu-id="0151d-1532">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1532">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="0151d-1533">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1533">Role</span></span>

* <span data-ttu-id="0151d-1534">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="0151d-1534">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0151d-1535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0151d-1535">Service Fabric</span></span>

* <span data-ttu-id="0151d-1536">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1536">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="0151d-1537">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1537">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1538">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1538">VM</span></span>

* <span data-ttu-id="0151d-1539">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="0151d-1539">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="0151d-1540">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1540">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="0151d-1541">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="0151d-1541">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="0151d-1542">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1542">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="0151d-1543">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1543">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="0151d-1544">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1544">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0151d-1545">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1545">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="0151d-1546">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1546">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="0151d-1547">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1547">December 19, 2017</span></span>

<span data-ttu-id="0151d-1548">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="0151d-1548">Version 2.0.23</span></span>

* <span data-ttu-id="0151d-1549">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1549">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1550">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1550">Container</span></span>

* <span data-ttu-id="0151d-1551">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1551">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1552">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1552">Network</span></span>

* <span data-ttu-id="0151d-1553">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1553">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="0151d-1554">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1554">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1555">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1555">Storage</span></span>

* <span data-ttu-id="0151d-1556">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1556">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1557">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1557">VM</span></span>

* <span data-ttu-id="0151d-1558">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1558">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="0151d-1559">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1559">December 5, 2017</span></span>

<span data-ttu-id="0151d-1560">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="0151d-1560">Version 2.0.22</span></span>

* <span data-ttu-id="0151d-1561">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1561">Removed `az component` commands.</span></span> <span data-ttu-id="0151d-1562">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1562">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1563">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1563">Core</span></span>
* <span data-ttu-id="0151d-1564">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="0151d-1564">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="0151d-1565">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1565">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1566">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1566">ACS</span></span>

* <span data-ttu-id="0151d-1567">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1567">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="0151d-1568">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="0151d-1568">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="0151d-1569">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="0151d-1569">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="0151d-1570">Advisor</span><span class="sxs-lookup"><span data-stu-id="0151d-1570">Advisor</span></span>

* <span data-ttu-id="0151d-1571">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1571">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1572">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1572">Appservice</span></span>

* <span data-ttu-id="0151d-1573">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="0151d-1573">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="0151d-1574">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0151d-1574">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="0151d-1575">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1575">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="0151d-1576">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0151d-1576">Consumption</span></span>

* <span data-ttu-id="0151d-1577">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1577">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1578">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1578">Container</span></span>

* <span data-ttu-id="0151d-1579">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="0151d-1579">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1580">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1580">Monitor</span></span>

* <span data-ttu-id="0151d-1581">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1581">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1582">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1582">Resource</span></span>

* <span data-ttu-id="0151d-1583">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1583">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="0151d-1584">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-1584">Role</span></span>

* <span data-ttu-id="0151d-1585">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1585">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="0151d-1586">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1586">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="0151d-1587">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0151d-1587">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1588">SQL</span></span>

* <span data-ttu-id="0151d-1589">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1589">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="0151d-1590">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1590">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1591">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1591">VM</span></span>

* <span data-ttu-id="0151d-1592">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1592">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="0151d-1593">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1593">November 14, 2017</span></span>

<span data-ttu-id="0151d-1594">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="0151d-1594">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1595">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1595">ACR</span></span>

* <span data-ttu-id="0151d-1596">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1596">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="0151d-1597">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1597">ACS</span></span>

* <span data-ttu-id="0151d-1598">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1598">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="0151d-1599">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0151d-1599">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="0151d-1600">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="0151d-1600">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="0151d-1601">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1601">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="0151d-1602">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1602">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1603">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1603">Appservice</span></span>

* <span data-ttu-id="0151d-1604">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1604">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="0151d-1605">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1605">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="0151d-1606">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1606">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="0151d-1607">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1607">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="0151d-1608">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1608">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="0151d-1609">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0151d-1609">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1610">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1610">Batch</span></span>

* <span data-ttu-id="0151d-1611">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0151d-1611">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="0151d-1612">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0151d-1612">Batchai</span></span>

* <span data-ttu-id="0151d-1613">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1613">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="0151d-1614">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1614">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="0151d-1615">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1615">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="0151d-1616">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1616">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="0151d-1617">Cloud</span><span class="sxs-lookup"><span data-stu-id="0151d-1617">Cloud</span></span>

* <span data-ttu-id="0151d-1618">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="0151d-1618">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1619">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1619">Container</span></span>

* <span data-ttu-id="0151d-1620">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1620">Added support to open multiple ports</span></span>
* <span data-ttu-id="0151d-1621">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1621">Added container group restart policy</span></span>
* <span data-ttu-id="0151d-1622">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1622">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="0151d-1623">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1623">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0151d-1624">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0151d-1624">Data Lake Analytics</span></span>

* <span data-ttu-id="0151d-1625">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="0151d-1625">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0151d-1626">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0151d-1626">Data Lake Store</span></span>

* <span data-ttu-id="0151d-1627">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="0151d-1627">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1628">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1628">Extension</span></span>

* <span data-ttu-id="0151d-1629">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1629">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="0151d-1630">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0151d-1630">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1631">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1631">IoT</span></span>

* <span data-ttu-id="0151d-1632">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1632">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1633">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1633">Monitor</span></span>

* <span data-ttu-id="0151d-1634">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1634">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1635">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1635">Network</span></span>

* <span data-ttu-id="0151d-1636">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1636">Added support for CAA DNS records</span></span>
* <span data-ttu-id="0151d-1637">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="0151d-1637">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="0151d-1638">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0151d-1638">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="0151d-1639">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1639">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="0151d-1640">Reservations</span><span class="sxs-lookup"><span data-stu-id="0151d-1640">Reservations</span></span>

* <span data-ttu-id="0151d-1641">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0151d-1641">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1642">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1642">Resource</span></span>

* <span data-ttu-id="0151d-1643">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1643">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1644">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1644">SQL</span></span>

* <span data-ttu-id="0151d-1645">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1645">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1646">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1646">Storage</span></span>

* <span data-ttu-id="0151d-1647">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1647">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="0151d-1648">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="0151d-1648">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="0151d-1649">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0151d-1649">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="0151d-1650">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1650">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="0151d-1651">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1651">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="0151d-1652">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1652">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="0151d-1653">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1653">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1654">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1654">VM</span></span>

* <span data-ttu-id="0151d-1655">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0151d-1655">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="0151d-1656">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1656">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="0151d-1657">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="0151d-1657">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="0151d-1658">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1658">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="0151d-1659">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1659">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="0151d-1660">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1660">October 24, 2017</span></span>

<span data-ttu-id="0151d-1661">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="0151d-1661">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1662">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1662">Core</span></span>

* <span data-ttu-id="0151d-1663">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="0151d-1663">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1664">ACR</span></span>

* <span data-ttu-id="0151d-1665">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1665">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="0151d-1666">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="0151d-1666">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="0151d-1667">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1667">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1668">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1668">ACS</span></span>

* <span data-ttu-id="0151d-1669">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1669">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="0151d-1670">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1670">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1671">Appservice</span></span>

* <span data-ttu-id="0151d-1672">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="0151d-1672">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="0151d-1673">Komponente</span><span class="sxs-lookup"><span data-stu-id="0151d-1673">Component</span></span>

* <span data-ttu-id="0151d-1674">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1674">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1675">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1675">Monitor</span></span>

* <span data-ttu-id="0151d-1676">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1676">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1677">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1677">Resource</span></span>

* <span data-ttu-id="0151d-1678">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1678">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="0151d-1679">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="0151d-1679">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1680">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1680">VM</span></span>

* <span data-ttu-id="0151d-1681">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1681">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="0151d-1682">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1682">October 9, 2017</span></span>

<span data-ttu-id="0151d-1683">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="0151d-1683">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1684">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1684">Core</span></span>

* <span data-ttu-id="0151d-1685">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1685">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1686">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1686">Appservice</span></span>

* <span data-ttu-id="0151d-1687">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1687">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1688">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1688">Batch</span></span>

* <span data-ttu-id="0151d-1689">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="0151d-1689">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="0151d-1690">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1690">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="0151d-1691">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1691">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="0151d-1692">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1692">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="0151d-1693">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0151d-1693">Batchai</span></span>

* <span data-ttu-id="0151d-1694">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-1694">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-1695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-1695">Keyvault</span></span>

* <span data-ttu-id="0151d-1696">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="0151d-1696">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="0151d-1697">(#4448)</span><span class="sxs-lookup"><span data-stu-id="0151d-1697">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="0151d-1698">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1698">Network</span></span>

* <span data-ttu-id="0151d-1699">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="0151d-1699">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="0151d-1700">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1700">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1701">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1701">Resource</span></span>

* <span data-ttu-id="0151d-1702">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1702">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="0151d-1703">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1703">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="0151d-1704">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1704">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="0151d-1705">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1705">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1706">Sql</span><span class="sxs-lookup"><span data-stu-id="0151d-1706">Sql</span></span>

* <span data-ttu-id="0151d-1707">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1707">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="0151d-1708">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1708">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="0151d-1709">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1709">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1710">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1710">Storage</span></span>

* <span data-ttu-id="0151d-1711">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1711">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1712">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1712">Vm</span></span>

* <span data-ttu-id="0151d-1713">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="0151d-1713">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="0151d-1714">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1714">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="0151d-1715">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1715">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="0151d-1716">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1716">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="0151d-1717">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1717">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="0151d-1718">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1718">September 22, 2017</span></span>

<span data-ttu-id="0151d-1719">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="0151d-1719">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1720">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1720">Resource</span></span>

* <span data-ttu-id="0151d-1721">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1721">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="0151d-1722">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1722">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="0151d-1723">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1723">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="0151d-1724">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="0151d-1724">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1725">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1725">Network</span></span>

* <span data-ttu-id="0151d-1726">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1726">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="0151d-1727">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1727">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="0151d-1728">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1728">Added `asg` application security group commands</span></span>
* <span data-ttu-id="0151d-1729">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1729">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="0151d-1730">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1730">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0151d-1731">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1731">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="0151d-1732">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1732">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1733">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1733">Storage</span></span>

* <span data-ttu-id="0151d-1734">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0151d-1734">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0151d-1735">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="0151d-1735">Eventgrid</span></span>

* <span data-ttu-id="0151d-1736">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1736">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1737">SQL</span></span>

* <span data-ttu-id="0151d-1738">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="0151d-1738">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="0151d-1739">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0151d-1739">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="0151d-1740">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1740">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-1741">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-1741">Keyvault</span></span>

* <span data-ttu-id="0151d-1742">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1742">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1743">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1743">VM</span></span>

* <span data-ttu-id="0151d-1744">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1744">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="0151d-1745">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0151d-1745">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="0151d-1746">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1746">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="0151d-1747">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1747">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="0151d-1748">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1748">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="0151d-1749">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1749">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1750">ACS</span></span>

* <span data-ttu-id="0151d-1751">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1751">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1752">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1752">Appservice</span></span>

* <span data-ttu-id="0151d-1753">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="0151d-1753">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0151d-1754">Backup</span><span class="sxs-lookup"><span data-stu-id="0151d-1754">Backup</span></span>

* <span data-ttu-id="0151d-1755">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0151d-1755">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="0151d-1756">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1756">September 11, 2017</span></span>

<span data-ttu-id="0151d-1757">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0151d-1757">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0151d-1758">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1758">Core</span></span>

* <span data-ttu-id="0151d-1759">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="0151d-1759">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0151d-1760">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="0151d-1760">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1761">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1761">Acs</span></span>

* <span data-ttu-id="0151d-1762">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1762">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0151d-1763">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="0151d-1763">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1764">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1764">Appservice</span></span>

* <span data-ttu-id="0151d-1765">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="0151d-1765">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0151d-1766">CDN</span><span class="sxs-lookup"><span data-stu-id="0151d-1766">CDN</span></span>

* <span data-ttu-id="0151d-1767">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0151d-1767">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="0151d-1768">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0151d-1768">Extension</span></span>

* <span data-ttu-id="0151d-1769">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1769">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-1770">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-1770">Keyvault</span></span>

* <span data-ttu-id="0151d-1771">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="0151d-1771">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1772">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1772">Network</span></span>

* <span data-ttu-id="0151d-1773">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1773">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0151d-1774">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1774">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0151d-1775">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1775">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0151d-1776">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1776">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0151d-1777">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1777">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-1778">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-1778">Resource</span></span>

* <span data-ttu-id="0151d-1779">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="0151d-1779">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0151d-1780">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="0151d-1780">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0151d-1781">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="0151d-1781">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0151d-1782">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1782">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-1783">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-1783">SQL</span></span>

* <span data-ttu-id="0151d-1784">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1784">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1785">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1785">VM</span></span>

* <span data-ttu-id="0151d-1786">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1786">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0151d-1787">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="0151d-1787">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0151d-1788">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1788">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0151d-1789">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="0151d-1789">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0151d-1790">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="0151d-1790">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0151d-1791">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1791">August 31, 2017</span></span>

<span data-ttu-id="0151d-1792">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0151d-1792">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-1793">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-1793">Keyvault</span></span>

* <span data-ttu-id="0151d-1794">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="0151d-1794">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0151d-1795">Sf</span><span class="sxs-lookup"><span data-stu-id="0151d-1795">Sf</span></span>

* <span data-ttu-id="0151d-1796">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1796">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1797">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1797">Storage</span></span>

* <span data-ttu-id="0151d-1798">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="0151d-1798">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0151d-1799">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="0151d-1799">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0151d-1800">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1800">August 28, 2017</span></span>

<span data-ttu-id="0151d-1801">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0151d-1801">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0151d-1802">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="0151d-1802">CLI</span></span>

* <span data-ttu-id="0151d-1803">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1803">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1804">ACS</span></span>

* <span data-ttu-id="0151d-1805">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1805">Corrected preview regions</span></span>
* <span data-ttu-id="0151d-1806">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1806">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="0151d-1807">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1807">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1808">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1808">Appservice</span></span>

* <span data-ttu-id="0151d-1809">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1809">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0151d-1810">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1810">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0151d-1811">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1811">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0151d-1812">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="0151d-1812">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0151d-1813">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="0151d-1813">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1814">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1814">IoT</span></span>

* <span data-ttu-id="0151d-1815">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="0151d-1815">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1816">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1816">Network</span></span>

* <span data-ttu-id="0151d-1817">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1817">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0151d-1818">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1818">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0151d-1819">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1819">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0151d-1820">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1820">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0151d-1821">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1821">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1822">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1822">Profile</span></span>

* <span data-ttu-id="0151d-1823">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1823">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0151d-1824">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0151d-1824">Service Fabric</span></span>

* <span data-ttu-id="0151d-1825">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0151d-1825">Preview release</span></span>
* <span data-ttu-id="0151d-1826">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1826">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0151d-1827">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1827">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0151d-1828">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1828">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1829">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1829">Storage</span></span>

* <span data-ttu-id="0151d-1830">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-1830">Enabled setting blob tier</span></span>
* <span data-ttu-id="0151d-1831">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1831">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0151d-1832">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1832">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="0151d-1833">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-1833">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0151d-1834">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1834">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0151d-1835">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="0151d-1835">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1836">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1836">VM</span></span>

* <span data-ttu-id="0151d-1837">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1837">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0151d-1838">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1838">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="0151d-1839">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1839">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="0151d-1840">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="0151d-1840">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0151d-1841">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1841">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0151d-1842">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-1842">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0151d-1843">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1843">August 15, 2017</span></span>

<span data-ttu-id="0151d-1844">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0151d-1844">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1845">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1845">ACS</span></span>

* <span data-ttu-id="0151d-1846">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1846">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1847">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1847">Appservice</span></span>

* <span data-ttu-id="0151d-1848">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1848">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0151d-1849">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0151d-1849">Event Grid</span></span>

* <span data-ttu-id="0151d-1850">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1850">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0151d-1851">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1851">August 11, 2017</span></span>

<span data-ttu-id="0151d-1852">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0151d-1852">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1853">ACS</span></span>

* <span data-ttu-id="0151d-1854">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1854">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1855">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1855">Batch</span></span>

* <span data-ttu-id="0151d-1856">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1856">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0151d-1857">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1857">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0151d-1858">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1858">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0151d-1859">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="0151d-1859">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0151d-1860">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="0151d-1860">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0151d-1861">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1861">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0151d-1862">Komponente</span><span class="sxs-lookup"><span data-stu-id="0151d-1862">Component</span></span>

* <span data-ttu-id="0151d-1863">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1863">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0151d-1864">Container</span><span class="sxs-lookup"><span data-stu-id="0151d-1864">Container</span></span>

* <span data-ttu-id="0151d-1865">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="0151d-1865">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0151d-1866">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0151d-1866">Data Lake Store</span></span>

* <span data-ttu-id="0151d-1867">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-1867">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0151d-1868">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0151d-1868">Event Grid</span></span>

* <span data-ttu-id="0151d-1869">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0151d-1869">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1870">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1870">Network</span></span>

* <span data-ttu-id="0151d-1871">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-1871">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0151d-1872">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-1872">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0151d-1873">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-1873">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0151d-1874">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="0151d-1874">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-1875">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1875">Profile</span></span>

* <span data-ttu-id="0151d-1876">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="0151d-1876">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-1877">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-1877">Storage</span></span>

* <span data-ttu-id="0151d-1878">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-1878">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-1879">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-1879">VM</span></span>

* <span data-ttu-id="0151d-1880">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1880">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0151d-1881">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1881">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0151d-1882">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="0151d-1882">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0151d-1883">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="0151d-1883">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0151d-1884">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1884">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0151d-1885">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-1885">July 28, 2017</span></span>

<span data-ttu-id="0151d-1886">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0151d-1886">Version 2.0.12</span></span>

* <span data-ttu-id="0151d-1887">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1887">Added container commands</span></span>
* <span data-ttu-id="0151d-1888">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1888">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="0151d-1889">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-1889">Core</span></span>

* <span data-ttu-id="0151d-1890">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="0151d-1890">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0151d-1891">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1891">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0151d-1892">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="0151d-1892">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0151d-1893">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="0151d-1893">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0151d-1894">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="0151d-1894">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0151d-1895">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="0151d-1895">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0151d-1896">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="0151d-1896">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0151d-1897">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="0151d-1897">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0151d-1898">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="0151d-1898">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0151d-1899">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-1899">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0151d-1900">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="0151d-1900">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0151d-1901">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="0151d-1901">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0151d-1902">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="0151d-1902">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0151d-1903">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="0151d-1903">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0151d-1904">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="0151d-1904">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0151d-1905">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="0151d-1905">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0151d-1906">ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1906">ACR</span></span>

* <span data-ttu-id="0151d-1907">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1907">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0151d-1908">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="0151d-1908">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0151d-1909">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1909">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0151d-1910">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1910">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0151d-1911">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1911">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0151d-1912">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1912">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-1913">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-1913">ACS</span></span>

* <span data-ttu-id="0151d-1914">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="0151d-1914">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-1915">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-1915">Appservice</span></span>

* <span data-ttu-id="0151d-1916">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="0151d-1916">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0151d-1917">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="0151d-1917">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0151d-1918">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="0151d-1918">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0151d-1919">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="0151d-1919">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0151d-1920">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="0151d-1920">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0151d-1921">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="0151d-1921">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0151d-1922">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="0151d-1922">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0151d-1923">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="0151d-1923">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0151d-1924">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1924">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0151d-1925">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="0151d-1925">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0151d-1926">Batch</span><span class="sxs-lookup"><span data-stu-id="0151d-1926">Batch</span></span>

* <span data-ttu-id="0151d-1927">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1927">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0151d-1928">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1928">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0151d-1929">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1929">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0151d-1930">CDN</span><span class="sxs-lookup"><span data-stu-id="0151d-1930">CDN</span></span>

* <span data-ttu-id="0151d-1931">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0151d-1931">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="0151d-1932">Cloud</span><span class="sxs-lookup"><span data-stu-id="0151d-1932">Cloud</span></span>

* <span data-ttu-id="0151d-1933">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="0151d-1933">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0151d-1934">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="0151d-1934">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0151d-1935">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0151d-1935">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0151d-1936">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="0151d-1936">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0151d-1937">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0151d-1937">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-1938">CosmosDB</span></span>

* <span data-ttu-id="0151d-1939">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="0151d-1939">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0151d-1940">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1940">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0151d-1941">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0151d-1941">Data Lake Analytics</span></span>

* <span data-ttu-id="0151d-1942">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1942">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0151d-1943">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1943">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0151d-1944">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1944">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0151d-1945">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0151d-1945">Data Lake Store</span></span>

* <span data-ttu-id="0151d-1946">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1946">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0151d-1947">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="0151d-1947">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0151d-1948">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1948">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0151d-1949">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="0151d-1949">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0151d-1950">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="0151d-1950">Interactive</span></span>

* <span data-ttu-id="0151d-1951">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1951">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0151d-1952">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-1952">Increased test coverage</span></span>
* <span data-ttu-id="0151d-1953">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-1953">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0151d-1954">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="0151d-1954">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0151d-1955">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="0151d-1955">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0151d-1956">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="0151d-1956">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0151d-1957">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="0151d-1957">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0151d-1958">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1958">Added `--progress` flag</span></span>
* <span data-ttu-id="0151d-1959">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-1959">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0151d-1960">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="0151d-1960">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0151d-1961">IoT</span><span class="sxs-lookup"><span data-stu-id="0151d-1961">IoT</span></span>

* <span data-ttu-id="0151d-1962">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="0151d-1962">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0151d-1963">(3934)</span><span class="sxs-lookup"><span data-stu-id="0151d-1963">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0151d-1964">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="0151d-1964">Key vault</span></span>

* <span data-ttu-id="0151d-1965">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0151d-1965">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0151d-1966">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0151d-1966">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0151d-1967">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0151d-1967">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0151d-1968">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0151d-1968">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0151d-1969">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0151d-1969">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0151d-1970">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="0151d-1970">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0151d-1971">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0151d-1971">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0151d-1972">(3307)</span><span class="sxs-lookup"><span data-stu-id="0151d-1972">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0151d-1973">Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-1973">Lab</span></span>

* <span data-ttu-id="0151d-1974">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1974">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0151d-1975">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1975">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-1976">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-1976">Monitor</span></span>

* <span data-ttu-id="0151d-1977">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="0151d-1977">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0151d-1978">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1978">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0151d-1979">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1979">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0151d-1980">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1980">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0151d-1981">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0151d-1981">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0151d-1982">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="0151d-1982">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0151d-1983">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="0151d-1983">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0151d-1984">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="0151d-1984">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0151d-1985">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="0151d-1985">`location` no longer required</span></span>
  * <span data-ttu-id="0151d-1986">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="0151d-1986">Add name and ID support for target</span></span>
  * <span data-ttu-id="0151d-1987">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="0151d-1987">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0151d-1988">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="0151d-1988">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0151d-1989">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0151d-1989">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0151d-1990">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="0151d-1990">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0151d-1991">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="0151d-1991">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0151d-1992">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1992">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0151d-1993">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-1993">Network</span></span>

* <span data-ttu-id="0151d-1994">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1994">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0151d-1995">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1995">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0151d-1996">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0151d-1996">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0151d-1997">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0151d-1997">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0151d-1998">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0151d-1998">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0151d-1999">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-1999">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0151d-2000">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0151d-2000">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0151d-2001">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0151d-2001">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0151d-2002">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0151d-2002">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0151d-2003">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0151d-2003">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0151d-2004">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2004">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0151d-2005">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2005">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0151d-2006">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0151d-2006">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0151d-2007">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2007">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0151d-2008">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2008">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0151d-2009">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-2009">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0151d-2010">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="0151d-2010">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0151d-2011">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-2011">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0151d-2012">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2012">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0151d-2013">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-2013">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0151d-2014">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="0151d-2014">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0151d-2015">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0151d-2015">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0151d-2016">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-2016">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0151d-2017">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0151d-2017">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0151d-2018">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0151d-2018">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0151d-2019">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0151d-2019">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0151d-2020">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0151d-2020">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-2021">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-2021">Profile</span></span>

* <span data-ttu-id="0151d-2022">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="0151d-2022">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0151d-2023">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="0151d-2023">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0151d-2024">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="0151d-2024">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0151d-2025">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2025">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0151d-2026">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="0151d-2026">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0151d-2027">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0151d-2027">RDBMS</span></span>

* <span data-ttu-id="0151d-2028">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="0151d-2028">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0151d-2029">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="0151d-2029">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0151d-2030">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="0151d-2030">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0151d-2031">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="0151d-2031">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-2032">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-2032">Resource</span></span>

* <span data-ttu-id="0151d-2033">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-2033">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0151d-2034">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="0151d-2034">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0151d-2035">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-2035">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0151d-2036">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="0151d-2036">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0151d-2037">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="0151d-2037">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0151d-2038">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="0151d-2038">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0151d-2039">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="0151d-2039">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0151d-2040">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2040">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0151d-2041">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-2041">Role</span></span>

* <span data-ttu-id="0151d-2042">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0151d-2042">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0151d-2043">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="0151d-2043">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0151d-2044">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="0151d-2044">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0151d-2045">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="0151d-2045">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0151d-2046">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2046">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0151d-2047">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0151d-2047">Service Fabric</span></span>
* <span data-ttu-id="0151d-2048">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="0151d-2048">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0151d-2049">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="0151d-2049">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0151d-2050">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="0151d-2050">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-2051">SQL</span></span>

* <span data-ttu-id="0151d-2052">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-2052">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0151d-2053">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0151d-2053">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0151d-2054">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2054">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-2055">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-2055">Storage</span></span>

* <span data-ttu-id="0151d-2056">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="0151d-2056">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0151d-2057">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0151d-2057">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0151d-2058">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="0151d-2058">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0151d-2059">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="0151d-2059">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="0151d-2060">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="0151d-2060">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="0151d-2061">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="0151d-2061">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-2062">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-2062">VM</span></span>

* <span data-ttu-id="0151d-2063">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="0151d-2063">Support configuring nsg</span></span>
* <span data-ttu-id="0151d-2064">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-2064">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0151d-2065">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="0151d-2065">Support managed service identities</span></span>
* <span data-ttu-id="0151d-2066">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="0151d-2066">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="0151d-2067">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="0151d-2067">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0151d-2068">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-2068">May 10, 2017</span></span>

<span data-ttu-id="0151d-2069">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0151d-2069">Version 2.0.6</span></span>

* <span data-ttu-id="0151d-2070">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="0151d-2070">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0151d-2071">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="0151d-2071">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0151d-2072">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="0151d-2072">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="0151d-2073">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-2073">Include Cognitive Services module</span></span>
* <span data-ttu-id="0151d-2074">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-2074">Include Service Fabric module</span></span>
* <span data-ttu-id="0151d-2075">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="0151d-2075">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="0151d-2076">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="0151d-2076">Add support for CDN commands</span></span>
* <span data-ttu-id="0151d-2077">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="0151d-2077">Remove Container module</span></span>
* <span data-ttu-id="0151d-2078">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="0151d-2078">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0151d-2079">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0151d-2079">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="0151d-2080">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-2080">Core</span></span>

* <span data-ttu-id="0151d-2081">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="0151d-2081">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="0151d-2082">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0151d-2082">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0151d-2083">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0151d-2083">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0151d-2084">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0151d-2084">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0151d-2085">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0151d-2085">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0151d-2086">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0151d-2086">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0151d-2087">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0151d-2087">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0151d-2088">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0151d-2088">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0151d-2089">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0151d-2089">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0151d-2090">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="0151d-2090">core: Improved performance</span></span>
* <span data-ttu-id="0151d-2091">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="0151d-2091">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0151d-2092">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="0151d-2092">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-2093">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-2093">ACS</span></span>

* <span data-ttu-id="0151d-2094">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0151d-2094">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0151d-2095">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="0151d-2095">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0151d-2096">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="0151d-2096">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0151d-2097">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0151d-2097">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-2098">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-2098">AppService</span></span>

* <span data-ttu-id="0151d-2099">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="0151d-2099">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0151d-2100">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="0151d-2100">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0151d-2101">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="0151d-2101">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0151d-2102">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="0151d-2102">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0151d-2103">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="0151d-2103">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0151d-2104">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0151d-2104">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0151d-2105">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="0151d-2105">support slot swap with preview</span></span>
* <span data-ttu-id="0151d-2106">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0151d-2106">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0151d-2107">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0151d-2107">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0151d-2108">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0151d-2108">CosmosDB</span></span>

* <span data-ttu-id="0151d-2109">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="0151d-2109">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="0151d-2110">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="0151d-2110">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0151d-2111">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="0151d-2111">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0151d-2112">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="0151d-2112">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0151d-2113">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0151d-2113">Data Lake Analytics</span></span>

* <span data-ttu-id="0151d-2114">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="0151d-2114">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="0151d-2115">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="0151d-2115">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0151d-2116">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="0151d-2116">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0151d-2117">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="0151d-2117">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0151d-2118">Table</span><span class="sxs-lookup"><span data-stu-id="0151d-2118">Table</span></span>
  * <span data-ttu-id="0151d-2119">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="0151d-2119">Table valued function</span></span>
  * <span data-ttu-id="0151d-2120">Sicht</span><span class="sxs-lookup"><span data-stu-id="0151d-2120">View</span></span>
  * <span data-ttu-id="0151d-2121">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="0151d-2121">Table Statistics.</span></span> <span data-ttu-id="0151d-2122">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="0151d-2122">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0151d-2123">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0151d-2123">Data Lake Store</span></span>

* <span data-ttu-id="0151d-2124">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-2124">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="0151d-2125">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0151d-2125">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0151d-2126">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="0151d-2126">missed help for access show.</span></span> <span data-ttu-id="0151d-2127">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0151d-2127">adding it.</span></span> <span data-ttu-id="0151d-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0151d-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0151d-2129">Suchen</span><span class="sxs-lookup"><span data-stu-id="0151d-2129">Find</span></span>

* <span data-ttu-id="0151d-2130">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="0151d-2130">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0151d-2131">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0151d-2131">KeyVault</span></span>

* <span data-ttu-id="0151d-2132">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="0151d-2132">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0151d-2133">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="0151d-2133">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="0151d-2134">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="0151d-2134">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0151d-2135">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="0151d-2135">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="0151d-2136">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0151d-2136">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0151d-2137">Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-2137">Lab</span></span>

* <span data-ttu-id="0151d-2138">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="0151d-2138">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="0151d-2139">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-2139">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="0151d-2140">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="0151d-2140">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="0151d-2141">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="0151d-2141">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="0151d-2142">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="0151d-2142">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="0151d-2143">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0151d-2143">Monitor</span></span>

* <span data-ttu-id="0151d-2144">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0151d-2144">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0151d-2145">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0151d-2145">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0151d-2146">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-2146">Network</span></span>

* <span data-ttu-id="0151d-2147">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="0151d-2147">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="0151d-2148">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="0151d-2148">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="0151d-2149">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="0151d-2149">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="0151d-2150">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="0151d-2150">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="0151d-2151">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="0151d-2151">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="0151d-2152">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="0151d-2152">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="0151d-2153">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="0151d-2153">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="0151d-2154">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="0151d-2154">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="0151d-2155">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="0151d-2155">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="0151d-2156">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="0151d-2156">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0151d-2157">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="0151d-2157">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="0151d-2158">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="0151d-2158">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="0151d-2159">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="0151d-2159">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="0151d-2160">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0151d-2160">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="0151d-2161">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0151d-2161">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="0151d-2162">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="0151d-2162">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="0151d-2163">Profil</span><span class="sxs-lookup"><span data-stu-id="0151d-2163">Profile</span></span>

* <span data-ttu-id="0151d-2164">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0151d-2164">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0151d-2165">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0151d-2165">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0151d-2166">Redis</span><span class="sxs-lookup"><span data-stu-id="0151d-2166">Redis</span></span>

* <span data-ttu-id="0151d-2167">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="0151d-2167">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0151d-2168">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="0151d-2168">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="0151d-2169">Ressource</span><span class="sxs-lookup"><span data-stu-id="0151d-2169">Resource</span></span>

* <span data-ttu-id="0151d-2170">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0151d-2170">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0151d-2171">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0151d-2171">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0151d-2172">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0151d-2172">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0151d-2173">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="0151d-2173">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0151d-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0151d-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0151d-2175">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="0151d-2175">Add docs for az lock update.</span></span> <span data-ttu-id="0151d-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0151d-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0151d-2177">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="0151d-2177">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0151d-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0151d-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0151d-2179">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="0151d-2179">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0151d-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0151d-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0151d-2181">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0151d-2181">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0151d-2182">Rolle</span><span class="sxs-lookup"><span data-stu-id="0151d-2182">Role</span></span>

* <span data-ttu-id="0151d-2183">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0151d-2183">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0151d-2184">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0151d-2184">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0151d-2185">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0151d-2185">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0151d-2186">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="0151d-2186">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0151d-2187">SQL</span><span class="sxs-lookup"><span data-stu-id="0151d-2187">SQL</span></span>

* <span data-ttu-id="0151d-2188">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="0151d-2188">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="0151d-2189">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0151d-2189">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0151d-2190">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-2190">Storage</span></span>

* <span data-ttu-id="0151d-2191">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="0151d-2191">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="0151d-2192">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="0151d-2192">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0151d-2193">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="0151d-2193">Add support for large block blob upload</span></span>
* <span data-ttu-id="0151d-2194">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="0151d-2194">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-2195">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-2195">VM</span></span>

* <span data-ttu-id="0151d-2196">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="0151d-2196">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0151d-2197">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="0151d-2197">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0151d-2198">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0151d-2198">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0151d-2199">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0151d-2199">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0151d-2200">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="0151d-2200">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0151d-2201">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="0151d-2201">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0151d-2202">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0151d-2202">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0151d-2203">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-2203">April 3, 2017</span></span>

<span data-ttu-id="0151d-2204">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0151d-2204">Version 2.0.2</span></span>

<span data-ttu-id="0151d-2205">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="0151d-2205">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="0151d-2206">Core</span><span class="sxs-lookup"><span data-stu-id="0151d-2206">Core</span></span>

* <span data-ttu-id="0151d-2207">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="0151d-2207">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="0151d-2208">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0151d-2208">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0151d-2209">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0151d-2209">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0151d-2210">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0151d-2210">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0151d-2211">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0151d-2211">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0151d-2212">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="0151d-2212">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0151d-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0151d-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0151d-2214">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="0151d-2214">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0151d-2215">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="0151d-2215">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="0151d-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="0151d-2216">ACS</span></span>

* <span data-ttu-id="0151d-2217">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0151d-2217">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0151d-2218">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="0151d-2218">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0151d-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0151d-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0151d-2220">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="0151d-2220">Add support for windows clusters.</span></span> <span data-ttu-id="0151d-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0151d-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0151d-2222">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="0151d-2222">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0151d-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0151d-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="0151d-2224">AppService</span><span class="sxs-lookup"><span data-stu-id="0151d-2224">AppService</span></span>

* <span data-ttu-id="0151d-2225">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0151d-2225">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0151d-2226">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0151d-2226">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0151d-2227">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0151d-2227">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0151d-2228">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0151d-2228">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="0151d-2229">DataLake</span><span class="sxs-lookup"><span data-stu-id="0151d-2229">DataLake</span></span>

* <span data-ttu-id="0151d-2230">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-2230">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="0151d-2231">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="0151d-2231">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="0151d-2232">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="0151d-2232">DocuemntDB</span></span>

* <span data-ttu-id="0151d-2233">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0151d-2233">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0151d-2234">VM</span><span class="sxs-lookup"><span data-stu-id="0151d-2234">VM</span></span>

* <span data-ttu-id="0151d-2235">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0151d-2235">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0151d-2236">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0151d-2236">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0151d-2237">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0151d-2237">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0151d-2238">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0151d-2238">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0151d-2239">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0151d-2239">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0151d-2240">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="0151d-2240">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="0151d-2241">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0151d-2241">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0151d-2242">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="0151d-2242">February 27, 2017</span></span>

<span data-ttu-id="0151d-2243">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0151d-2243">Version 2.0.0</span></span>

<span data-ttu-id="0151d-2244">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="0151d-2244">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="0151d-2245">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="0151d-2245">Container Service (acs)</span></span>
- <span data-ttu-id="0151d-2246">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="0151d-2246">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0151d-2247">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0151d-2247">Networking</span></span>
- <span data-ttu-id="0151d-2248">Storage</span><span class="sxs-lookup"><span data-stu-id="0151d-2248">Storage</span></span>

<span data-ttu-id="0151d-2249">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="0151d-2249">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="0151d-2250">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="0151d-2250">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="0151d-2251">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="0151d-2251">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="0151d-2252">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="0151d-2252">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="0151d-2253">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="0151d-2253">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="0151d-2254">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="0151d-2254">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0151d-2255">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="0151d-2255">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0151d-2256">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="0151d-2256">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="0151d-2257">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="0151d-2257">Provide feedback from the command line with the `az feedback` command</span></span>


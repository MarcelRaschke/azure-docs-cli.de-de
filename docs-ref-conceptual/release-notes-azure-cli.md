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
ms.openlocfilehash: 9f35084eeecab491e5be63eb856b0bb64a6157d0
ms.sourcegitcommit: 9fb008f2802ca6a58f33e01263bf55a80d01f031
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/27/2019
ms.locfileid: "56891210"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="672ec-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="672ec-103">Azure CLI release notes</span></span>
## <a name="february-26-2019"></a><span data-ttu-id="672ec-104">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="672ec-104">February 26, 2019</span></span>

<span data-ttu-id="672ec-105">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="672ec-105">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="672ec-106">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-106">Core</span></span>

* <span data-ttu-id="672ec-107">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="672ec-107">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-108">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-108">ACR</span></span>

* <span data-ttu-id="672ec-109">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-109">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="672ec-110">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="672ec-110">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-111">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-111">ACS</span></span>

* <span data-ttu-id="672ec-112">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-112">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-113">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-113">AppService</span></span>

* <span data-ttu-id="672ec-114">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-114">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-115">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-115">Batch</span></span>
* <span data-ttu-id="672ec-116">[WICHTIGE ÄNDERUNG] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-116">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="672ec-117">[WICHTIGE ÄNDERUNG] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-117">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="672ec-118">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-118">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="672ec-119">[WICHTIGE ÄNDERUNG] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-119">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="672ec-120">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-120">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="672ec-121">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="672ec-121">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-122">CosmosDB</span></span>

* <span data-ttu-id="672ec-123">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-123">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="672ec-124">Kusto</span><span class="sxs-lookup"><span data-stu-id="672ec-124">Kusto</span></span>

* <span data-ttu-id="672ec-125">[WICHTIGE ÄNDERUNG] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-125">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="672ec-126">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-126">Network</span></span>

* <span data-ttu-id="672ec-127">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-127">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="672ec-128">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-128">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="672ec-129">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-129">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="672ec-130">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-130">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="672ec-131">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-131">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="672ec-132">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-132">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="672ec-133">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-133">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-134">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-134">Resource</span></span>

* <span data-ttu-id="672ec-135">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-135">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="672ec-136">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-136">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="672ec-137">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-137">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="672ec-138">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-138">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="672ec-139">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-139">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="672ec-140">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-140">Role</span></span>

* <span data-ttu-id="672ec-141">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-141">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-142">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-142">VM</span></span>

* <span data-ttu-id="672ec-143">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="672ec-143">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="672ec-144">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="672ec-144">February 12, 2019</span></span>

<span data-ttu-id="672ec-145">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="672ec-145">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="672ec-146">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-146">Core</span></span>

* <span data-ttu-id="672ec-147">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-147">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="672ec-148">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-148">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-149">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-149">ACR</span></span>
* <span data-ttu-id="672ec-150">[WICHTIGE ÄNDERUNG] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-150">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="672ec-151">[WICHTIGE ÄNDERUNG] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-151">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-152">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-152">ACS</span></span>
* <span data-ttu-id="672ec-153">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-153">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="672ec-154">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-154">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="672ec-155">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-155">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="672ec-156">AMS</span><span class="sxs-lookup"><span data-stu-id="672ec-156">AMS</span></span>
* <span data-ttu-id="672ec-157">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-157">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="672ec-158">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-158">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-159">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-159">Appservice</span></span>
* <span data-ttu-id="672ec-160">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-160">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="672ec-161">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-161">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="672ec-162">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="672ec-162">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="672ec-163">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-163">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="672ec-164">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-164">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="672ec-165">Botservice</span><span class="sxs-lookup"><span data-stu-id="672ec-165">Botservice</span></span>
* <span data-ttu-id="672ec-166">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="672ec-166">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="672ec-167">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-167">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="672ec-168">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-168">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="672ec-169">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="672ec-169">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="672ec-170">[VERALTET] Das `--proj-name`-Argument wurde zugunsten von `--proj-file-path` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-170">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="672ec-171">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="672ec-171">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="672ec-172">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-172">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="672ec-173">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-173">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="672ec-174">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="672ec-174">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="672ec-175">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="672ec-175">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="672ec-176">Key Vault</span><span class="sxs-lookup"><span data-stu-id="672ec-176">Key Vault</span></span>
* <span data-ttu-id="672ec-177">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="672ec-177">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-178">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-178">Monitor</span></span>
* <span data-ttu-id="672ec-179">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-179">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-180">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-180">Network</span></span>
* <span data-ttu-id="672ec-181">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="672ec-181">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="672ec-182">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="672ec-182">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="672ec-183">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="672ec-183">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="672ec-184">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-184">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="672ec-185">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="672ec-185">Policy Insights</span></span>
* <span data-ttu-id="672ec-186">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="672ec-186">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-187">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-187">RDBMS</span></span>
* <span data-ttu-id="672ec-188">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="672ec-188">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="672ec-189">Redis</span><span class="sxs-lookup"><span data-stu-id="672ec-189">Redis</span></span>
* <span data-ttu-id="672ec-190">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-190">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="672ec-191">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-191">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="672ec-192">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-192">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="672ec-193">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-193">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="672ec-194">[WICHTIGE ÄNDERUNG] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-194">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="672ec-195">[WICHTIGE ÄNDERUNG] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-195">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="672ec-196">[VERALTET] Warnmeldung für die Deaktivierung von des Befehls `redis import-method` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-196">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="672ec-197">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-197">Role</span></span>
* <span data-ttu-id="672ec-198">[WICHTIGE ÄNDERUNG] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-198">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="672ec-199">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="672ec-199">SQL VM</span></span>
* <span data-ttu-id="672ec-200">[VERALTET] Das `--boostrap-acc-pwd`-Argument wurde aufgrund eines Tippfehlers als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-200">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-201">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-201">VM</span></span>
* <span data-ttu-id="672ec-202">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="672ec-202">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="672ec-203">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-203">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="672ec-204">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="672ec-204">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="672ec-205">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-205">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="672ec-206">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="672ec-206">January 31, 2019</span></span>

<span data-ttu-id="672ec-207">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="672ec-207">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="672ec-208">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-208">Core</span></span>

* <span data-ttu-id="672ec-209">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="672ec-209">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="672ec-210">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="672ec-210">January 28, 2019</span></span>

<span data-ttu-id="672ec-211">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="672ec-211">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-212">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-212">ACR</span></span>
* <span data-ttu-id="672ec-213">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-213">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-214">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-214">ACS</span></span>
* <span data-ttu-id="672ec-215">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-215">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="672ec-216">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-216">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="672ec-217">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-217">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="672ec-218">AMS</span><span class="sxs-lookup"><span data-stu-id="672ec-218">AMS</span></span>
* <span data-ttu-id="672ec-219">[WICHTIGE ÄNDERUNG] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-219">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="672ec-220">[WICHTIGE ÄNDERUNG] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-220">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-221">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-221">Appservice</span></span>
* <span data-ttu-id="672ec-222">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-222">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="672ec-223">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-223">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="672ec-224">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-224">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="672ec-225">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-225">Container</span></span>
* <span data-ttu-id="672ec-226">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-226">Added `container start` command</span></span>
* <span data-ttu-id="672ec-227">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="672ec-227">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="672ec-228">EventGrid</span><span class="sxs-lookup"><span data-stu-id="672ec-228">EventGrid</span></span>
* <span data-ttu-id="672ec-229">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-229">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="672ec-230">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-230">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="672ec-231">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-231">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="672ec-232">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-232">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="672ec-233">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-233">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="672ec-234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="672ec-234">HDInsight</span></span>
* <span data-ttu-id="672ec-235">[WICHTIGE ÄNDERUNG] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-235">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="672ec-236">[WICHTIGE ÄNDERUNG] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-236">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="672ec-237">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-237">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="672ec-238">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-238">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="672ec-239">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-239">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="672ec-240">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-240">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-241">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-241">IoT</span></span>
* <span data-ttu-id="672ec-242">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-242">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="672ec-243">Kusto</span><span class="sxs-lookup"><span data-stu-id="672ec-243">Kusto</span></span>
* <span data-ttu-id="672ec-244">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="672ec-244">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-245">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-245">Monitor</span></span>
* <span data-ttu-id="672ec-246">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-246">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-247">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-247">Profile</span></span>
* <span data-ttu-id="672ec-248">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="672ec-248">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-249">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-249">Network</span></span>
* <span data-ttu-id="672ec-250">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="672ec-250">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="672ec-251">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="672ec-251">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-252">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-252">Resource</span></span>
* <span data-ttu-id="672ec-253">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-253">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="672ec-254">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-254">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="672ec-255">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="672ec-255">SQL Virtual Machine</span></span>
* <span data-ttu-id="672ec-256">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="672ec-256">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-257">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-257">Storage</span></span>
* <span data-ttu-id="672ec-258">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-258">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="672ec-259">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-259">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-260">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-260">VM</span></span>
* <span data-ttu-id="672ec-261">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-261">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="672ec-262">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-262">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="672ec-263">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="672ec-263">January 15, 2019</span></span>

<span data-ttu-id="672ec-264">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="672ec-264">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-265">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-265">ACR</span></span>
* <span data-ttu-id="672ec-266">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-266">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="672ec-267">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-267">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="672ec-268">[VERALTET] Parameter `--resource-group` wurde in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="672ec-268">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="672ec-269">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-269">ACS</span></span>
* <span data-ttu-id="672ec-270">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-270">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-271">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-271">Appservice</span></span>
* <span data-ttu-id="672ec-272">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="672ec-272">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="672ec-273">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-273">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="672ec-274">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-274">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="672ec-275">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-275">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="672ec-276">Botservice</span><span class="sxs-lookup"><span data-stu-id="672ec-276">Botservice</span></span>
* <span data-ttu-id="672ec-277">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-277">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="672ec-278">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="672ec-278">Configure</span></span>
* <span data-ttu-id="672ec-279">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-279">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-280">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-280">CosmosDB</span></span>
* <span data-ttu-id="672ec-281">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-281">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="672ec-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="672ec-282">HDInsight</span></span>
* <span data-ttu-id="672ec-283">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-283">Added commands for managing applications</span></span>
* <span data-ttu-id="672ec-284">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-284">Added commands for managing script actions</span></span>
* <span data-ttu-id="672ec-285">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-285">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="672ec-286">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-286">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="672ec-287">[WICHTIGE ÄNDERUNG] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-287">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-288">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-288">Network</span></span>
* <span data-ttu-id="672ec-289">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-289">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="672ec-290">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="672ec-290">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="672ec-291">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-291">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="672ec-292">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="672ec-292">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="672ec-293">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-293">Role</span></span>
* <span data-ttu-id="672ec-294">[VERALTET] Das `--password`-Argument wurde für `create-for-rbac` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-294">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="672ec-295">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="672ec-295">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="672ec-296">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="672ec-296">Security</span></span>
* <span data-ttu-id="672ec-297">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-297">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-298">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-298">Storage</span></span>
* <span data-ttu-id="672ec-299">[WICHTIGE ÄNDERUNG] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="672ec-299">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="672ec-300">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-300">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="672ec-301">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-301">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="672ec-302">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-302">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="672ec-303">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-303">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-304">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-304">VM</span></span>
* <span data-ttu-id="672ec-305">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="672ec-305">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="672ec-306">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-306">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="672ec-307">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-307">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="672ec-308">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="672ec-308">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="672ec-309">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="672ec-309">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="672ec-310">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="672ec-310">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="672ec-311">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-311">December 20, 2018</span></span>

<span data-ttu-id="672ec-312">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="672ec-312">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="672ec-313">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-313">Appservice</span></span>
* <span data-ttu-id="672ec-314">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-314">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="672ec-315">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-315">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="672ec-316">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-316">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="672ec-317">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="672ec-317">IoTCentral</span></span>
* <span data-ttu-id="672ec-318">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-318">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="672ec-319">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-319">Role</span></span>
* <span data-ttu-id="672ec-320">[WICHTIGE ÄNDERUNG] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="672ec-320">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-321">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-321">SQL</span></span>
* <span data-ttu-id="672ec-322">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-322">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-323">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-323">VM</span></span>
* <span data-ttu-id="672ec-324">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-324">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="672ec-325">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-325">December 18, 2018</span></span>

<span data-ttu-id="672ec-326">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="672ec-326">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="672ec-327">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-327">ACR</span></span>
* <span data-ttu-id="672ec-328">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-328">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="672ec-329">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="672ec-329">Condensed the table layout for task list</span></span>
* <span data-ttu-id="672ec-330">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-330">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-331">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-331">ACS</span></span>
* <span data-ttu-id="672ec-332">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-332">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="672ec-333">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-333">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="672ec-334">[VERALTET] `az acs`-Befehle als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="672ec-334">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="672ec-335">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="672ec-335">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="672ec-336">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-336">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="672ec-337">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-337">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-338">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-338">Appservice</span></span>
* <span data-ttu-id="672ec-339">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-339">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="672ec-340">Botservice</span><span class="sxs-lookup"><span data-stu-id="672ec-340">Botservice</span></span>
* <span data-ttu-id="672ec-341">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-341">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="672ec-342">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-342">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="672ec-343">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-343">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="672ec-344">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="672ec-344">Reduced Kudu network calls</span></span>
* <span data-ttu-id="672ec-345">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="672ec-345">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-346">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-346">Consumption</span></span>
* <span data-ttu-id="672ec-347">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-347">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-348">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-348">CosmosDB</span></span>
* <span data-ttu-id="672ec-349">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-349">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="672ec-350">Karten</span><span class="sxs-lookup"><span data-stu-id="672ec-350">Maps</span></span>
* <span data-ttu-id="672ec-351">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-351">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-352">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-352">Network</span></span>
* <span data-ttu-id="672ec-353">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-353">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="672ec-354">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="672ec-354">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-355">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-355">Resource</span></span>
* <span data-ttu-id="672ec-356">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-356">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="672ec-357">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-357">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-358">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-358">Storage</span></span>
*  <span data-ttu-id="672ec-359">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-359">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-360">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-360">VM</span></span>
* <span data-ttu-id="672ec-361">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="672ec-361">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="672ec-362">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-362">December 4, 2018</span></span>

<span data-ttu-id="672ec-363">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="672ec-363">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="672ec-364">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-364">Core</span></span>
* <span data-ttu-id="672ec-365">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-365">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="672ec-366">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-366">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-367">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-367">Appservice</span></span>
* <span data-ttu-id="672ec-368">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="672ec-368">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="672ec-369">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="672ec-369">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="672ec-370">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-370">Network</span></span>
* <span data-ttu-id="672ec-371">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-371">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="672ec-372">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-372">Role</span></span>
* <span data-ttu-id="672ec-373">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-373">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="672ec-374">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-374">VM</span></span>
* <span data-ttu-id="672ec-375">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-375">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="672ec-376">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="672ec-376">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="672ec-377">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="672ec-377">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="672ec-378">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="672ec-378">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="672ec-379">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-379">November 20, 2018</span></span>

<span data-ttu-id="672ec-380">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="672ec-380">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="672ec-381">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-381">Core</span></span>
* <span data-ttu-id="672ec-382">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-382">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-383">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-383">ACR</span></span>
* <span data-ttu-id="672ec-384">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-384">Added context token to task step</span></span>
* <span data-ttu-id="672ec-385">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-385">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="672ec-386">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-386">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-387">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-387">Appservice</span></span>
* <span data-ttu-id="672ec-388">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-388">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="672ec-389">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="672ec-389">Updated the default `node_version`.</span></span> <span data-ttu-id="672ec-390">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="672ec-390">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="672ec-391">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-391">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="672ec-392">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="672ec-392">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="672ec-393">IotCentral</span><span class="sxs-lookup"><span data-stu-id="672ec-393">IotCentral</span></span>
* <span data-ttu-id="672ec-394">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-394">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-395">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-395">KeyVault</span></span>
* <span data-ttu-id="672ec-396">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-396">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="672ec-397">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-397">Network</span></span>
* <span data-ttu-id="672ec-398">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-398">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="672ec-399">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-399">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="672ec-400">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-400">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="672ec-401">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-401">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-402">Rdbms</span><span class="sxs-lookup"><span data-stu-id="672ec-402">Rdbms</span></span>
* <span data-ttu-id="672ec-403">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-403">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="672ec-404">RBAC</span><span class="sxs-lookup"><span data-stu-id="672ec-404">Rbac</span></span>
* <span data-ttu-id="672ec-405">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-405">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="672ec-406">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-406">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="672ec-407">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-407">Storage</span></span>
* <span data-ttu-id="672ec-408">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-408">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="672ec-409">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="672ec-409">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="672ec-410">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-410">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="672ec-411">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-411">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-412">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-412">VM</span></span>
* <span data-ttu-id="672ec-413">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-413">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="672ec-414">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-414">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="672ec-415">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="672ec-415">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="672ec-416">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-416">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="672ec-417">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-417">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="672ec-418">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-418">Added `snapshot wait` command</span></span>
* <span data-ttu-id="672ec-419">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-419">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="672ec-420">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-420">November 6, 2018</span></span>

<span data-ttu-id="672ec-421">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="672ec-421">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="672ec-422">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-422">Core</span></span>
* <span data-ttu-id="672ec-423">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-423">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-424">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-424">ACR</span></span>
* <span data-ttu-id="672ec-425">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-425">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="672ec-426">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-426">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-427">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-427">ACS</span></span>
* <span data-ttu-id="672ec-428">[WICHTIGE ÄNDERUNG] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="672ec-428">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="672ec-429">Advisor</span><span class="sxs-lookup"><span data-stu-id="672ec-429">Advisor</span></span>
* <span data-ttu-id="672ec-430">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="672ec-430">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="672ec-431">AMS</span><span class="sxs-lookup"><span data-stu-id="672ec-431">AMS</span></span>
* <span data-ttu-id="672ec-432">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-432">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="672ec-433">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-433">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="672ec-434">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-434">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="672ec-435">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-435">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="672ec-436">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-436">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="672ec-437">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-437">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="672ec-438">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-438">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="672ec-439">[WICHTIGE ÄNDERUNG] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="672ec-439">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="672ec-440">[WICHTIGE ÄNDERUNG] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-440">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="672ec-441">[WICHTIGE ÄNDERUNG] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-441">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="672ec-442">[WICHTIGE ÄNDERUNG] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="672ec-442">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="672ec-443">[WICHTIGE ÄNDERUNG] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="672ec-443">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="672ec-444">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="672ec-444">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="672ec-445">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-445">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="672ec-446">[WICHTIGE ÄNDERUNG] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="672ec-446">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="672ec-447">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-447">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="672ec-448">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="672ec-448">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-449">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-449">AppService</span></span>
* <span data-ttu-id="672ec-450">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="672ec-450">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="672ec-451">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="672ec-451">Configure</span></span>
* <span data-ttu-id="672ec-452">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-452">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="672ec-453">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-453">Container</span></span>
* <span data-ttu-id="672ec-454">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="672ec-454">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="672ec-455">EventHub</span><span class="sxs-lookup"><span data-stu-id="672ec-455">EventHub</span></span>
* <span data-ttu-id="672ec-456">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-456">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-457">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-457">Interactive</span></span>
* <span data-ttu-id="672ec-458">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-458">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-459">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-459">Monitor</span></span>
* <span data-ttu-id="672ec-460">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-460">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-461">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-461">Network</span></span>
* <span data-ttu-id="672ec-462">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-462">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="672ec-463">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="672ec-463">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="672ec-464">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="672ec-464">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="672ec-465">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-465">Profile</span></span>
* <span data-ttu-id="672ec-466">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-466">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-467">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-467">RDBMS</span></span>
* <span data-ttu-id="672ec-468">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-468">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-469">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-469">Resource</span></span>
* <span data-ttu-id="672ec-470">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-470">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="672ec-471">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-471">Role</span></span>
* <span data-ttu-id="672ec-472">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-472">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="672ec-473">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="672ec-473">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="672ec-474">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-474">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-475">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-475">Storage</span></span>
* <span data-ttu-id="672ec-476">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="672ec-476">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-477">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-477">VM</span></span>
* <span data-ttu-id="672ec-478">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-478">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="672ec-479">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="672ec-479">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="672ec-480">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-480">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="672ec-481">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="672ec-481">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="672ec-482">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-482">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="672ec-483">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-483">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="672ec-484">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-484">October 23, 2018</span></span>

<span data-ttu-id="672ec-485">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="672ec-485">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="672ec-486">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-486">Core</span></span>
* <span data-ttu-id="672ec-487">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="672ec-487">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="672ec-488">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="672ec-488">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-489">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-489">ACR</span></span>
* <span data-ttu-id="672ec-490">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-490">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="672ec-491">CDN</span><span class="sxs-lookup"><span data-stu-id="672ec-491">CDN</span></span>
* <span data-ttu-id="672ec-492">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-492">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="672ec-493">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="672ec-493">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="672ec-494">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-494">Container</span></span>
* <span data-ttu-id="672ec-495">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-495">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="672ec-496">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="672ec-496">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="672ec-497">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-497">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="672ec-498">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="672ec-498">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="672ec-499">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="672ec-499">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="672ec-500">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-500">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="672ec-501">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-501">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-502">CosmosDB</span></span>
* <span data-ttu-id="672ec-503">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-503">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-504">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-504">Interactive</span></span>
* <span data-ttu-id="672ec-505">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-505">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="672ec-506">IoT Central</span><span class="sxs-lookup"><span data-stu-id="672ec-506">IoT Central</span></span>
* <span data-ttu-id="672ec-507">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-507">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="672ec-508">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="672ec-508">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-509">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-509">Monitor</span></span>
* <span data-ttu-id="672ec-510">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="672ec-510">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="672ec-511">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-511">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="672ec-512">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-512">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="672ec-513">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-513">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="672ec-514">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-514">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="672ec-515">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-515">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="672ec-516">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="672ec-516">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="672ec-517">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-517">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="672ec-518">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-518">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="672ec-519">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-519">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-520">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-520">Network</span></span>
* <span data-ttu-id="672ec-521">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-521">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="672ec-522">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-522">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="672ec-523">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="672ec-523">ServiceBus</span></span>
* <span data-ttu-id="672ec-524">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-524">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-525">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-525">SQL</span></span>
* <span data-ttu-id="672ec-526">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="672ec-526">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-527">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-527">Storage</span></span>
* <span data-ttu-id="672ec-528">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-528">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="672ec-529">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-529">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-530">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-530">VM</span></span>
* <span data-ttu-id="672ec-531">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="672ec-531">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="672ec-532">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-532">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="672ec-533">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-533">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="672ec-534">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-534">October 16, 2018</span></span>

<span data-ttu-id="672ec-535">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="672ec-535">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-536">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-536">VM</span></span>
* <span data-ttu-id="672ec-537">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="672ec-537">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="672ec-538">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-538">October 9, 2018</span></span>

<span data-ttu-id="672ec-539">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="672ec-539">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="672ec-540">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-540">Core</span></span>
* <span data-ttu-id="672ec-541">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="672ec-541">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-542">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-542">ACR</span></span>
* <span data-ttu-id="672ec-543">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-543">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-544">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-544">ACS</span></span>
* <span data-ttu-id="672ec-545">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="672ec-545">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="672ec-546">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="672ec-546">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="672ec-547">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="672ec-547">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="672ec-548">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="672ec-548">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="672ec-549">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-549">Container</span></span>
* <span data-ttu-id="672ec-550">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-550">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="672ec-551">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-551">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="672ec-552">Event Hub</span><span class="sxs-lookup"><span data-stu-id="672ec-552">Event Hub</span></span>
* <span data-ttu-id="672ec-553">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-553">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="672ec-554">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-554">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="672ec-555">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="672ec-555">Extensions</span></span>
* <span data-ttu-id="672ec-556">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="672ec-556">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="672ec-557">HDInsight</span><span class="sxs-lookup"><span data-stu-id="672ec-557">HDInsight</span></span>
* <span data-ttu-id="672ec-558">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-558">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-559">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-559">IoT</span></span>
* <span data-ttu-id="672ec-560">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-560">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-561">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-561">KeyVault</span></span>
* <span data-ttu-id="672ec-562">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="672ec-562">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="672ec-563">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-563">Network</span></span>
* <span data-ttu-id="672ec-564">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="672ec-564">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="672ec-565">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="672ec-565">See #6052</span></span>
* <span data-ttu-id="672ec-566">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="672ec-566">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="672ec-567">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="672ec-567">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="672ec-568">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-568">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="672ec-569">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-569">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="672ec-570">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="672ec-570">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="672ec-571">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-571">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="672ec-572">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-572">Role</span></span>
* <span data-ttu-id="672ec-573">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-573">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="672ec-574">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-574">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="672ec-575">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="672ec-575">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="672ec-576">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="672ec-576">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="672ec-577">Service Bus</span><span class="sxs-lookup"><span data-stu-id="672ec-577">Service Bus</span></span>
* <span data-ttu-id="672ec-578">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-578">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-579">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-579">VM</span></span>
* <span data-ttu-id="672ec-580">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-580">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="672ec-581">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="672ec-581">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="672ec-582">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-582">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="672ec-583">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-583">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="672ec-584">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-584">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="672ec-585">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-585">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="672ec-586">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-586">September 21, 2018</span></span>

<span data-ttu-id="672ec-587">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="672ec-587">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-588">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-588">ACR</span></span>
* <span data-ttu-id="672ec-589">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-589">Added ACR Task commands</span></span>
* <span data-ttu-id="672ec-590">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-590">Added quick run command</span></span>
* <span data-ttu-id="672ec-591">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-591">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="672ec-592">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-592">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="672ec-593">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-593">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="672ec-594">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-594">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-595">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-595">ACS</span></span>
* <span data-ttu-id="672ec-596">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-596">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="672ec-597">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-597">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-598">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-598">AppService</span></span>

* <span data-ttu-id="672ec-599">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="672ec-599">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="672ec-600">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-600">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="672ec-601">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-601">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="672ec-602">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-602">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-603">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-603">Batch</span></span>
* <span data-ttu-id="672ec-604">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-604">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="672ec-605">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-605">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="672ec-606">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-606">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="672ec-607">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-607">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="672ec-608">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-608">Batch AI</span></span> 
* <span data-ttu-id="672ec-609">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-609">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="672ec-610">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="672ec-610">Cognitive Services</span></span>
* <span data-ttu-id="672ec-611">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-611">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="672ec-612">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-612">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="672ec-613">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-613">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="672ec-614">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-614">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="672ec-615">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-615">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="672ec-616">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="672ec-616">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="672ec-617">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-617">Container</span></span>
* <span data-ttu-id="672ec-618">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-618">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="672ec-619">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-619">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="672ec-620">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-620">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="672ec-621">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-621">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="672ec-622">Data Lake</span><span class="sxs-lookup"><span data-stu-id="672ec-622">Datalake</span></span>
* <span data-ttu-id="672ec-623">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-623">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="672ec-624">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="672ec-624">Interactive Shell</span></span>
* <span data-ttu-id="672ec-625">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-625">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="672ec-626">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-626">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-627">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-627">IoT</span></span>
* <span data-ttu-id="672ec-628">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-628">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="672ec-629">Key Vault</span><span class="sxs-lookup"><span data-stu-id="672ec-629">Key Vault</span></span>
* <span data-ttu-id="672ec-630">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-630">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="672ec-631">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-631">Network</span></span>
* <span data-ttu-id="672ec-632">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-632">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="672ec-633">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-633">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="672ec-634">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-634">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="672ec-635">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-635">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="672ec-636">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-636">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="672ec-637">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-637">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="672ec-638">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-638">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="672ec-639">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="672ec-639">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="672ec-640">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-640">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="672ec-641">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-641">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="672ec-642">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-642">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="672ec-643">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-643">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="672ec-644">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-644">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="672ec-645">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="672ec-645">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="672ec-646">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-646">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="672ec-647">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="672ec-647">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="672ec-648">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-648">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="672ec-649">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-649">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-650">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-650">RDBMS</span></span>
* <span data-ttu-id="672ec-651">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-651">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="672ec-652">Reservierung</span><span class="sxs-lookup"><span data-stu-id="672ec-652">Reservation</span></span>
* <span data-ttu-id="672ec-653">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-653">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="672ec-654">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-654">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="672ec-655">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="672ec-655">Manage App</span></span>
* <span data-ttu-id="672ec-656">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="672ec-656">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="672ec-657">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="672ec-657">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="672ec-658">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-658">Role</span></span>
* <span data-ttu-id="672ec-659">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-659">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="672ec-660">SignalR</span><span class="sxs-lookup"><span data-stu-id="672ec-660">SignalR</span></span>
* <span data-ttu-id="672ec-661">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-661">First release</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-662">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-662">Storage</span></span>
* <span data-ttu-id="672ec-663">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-663">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="672ec-664">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-664">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-665">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-665">VM</span></span>
* <span data-ttu-id="672ec-666">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="672ec-666">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="672ec-667">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-667">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="672ec-668">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-668">August 28, 2018</span></span>

<span data-ttu-id="672ec-669">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="672ec-669">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="672ec-670">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-670">Core</span></span>

* <span data-ttu-id="672ec-671">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-671">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="672ec-672">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-672">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-673">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-673">ACR</span></span>

* <span data-ttu-id="672ec-674">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-674">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="672ec-675">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="672ec-675">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-676">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-676">ACS</span></span>

* <span data-ttu-id="672ec-677">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-677">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="672ec-678">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="672ec-678">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-679">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-679">AppService</span></span>

* <span data-ttu-id="672ec-680">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-680">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="672ec-681">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-681">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="672ec-682">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-682">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="672ec-683">Backup</span><span class="sxs-lookup"><span data-stu-id="672ec-683">Backup</span></span>

* <span data-ttu-id="672ec-684">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-684">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="672ec-685">Botdienst</span><span class="sxs-lookup"><span data-stu-id="672ec-685">Bot Service</span></span>

* <span data-ttu-id="672ec-686">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="672ec-686">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="672ec-687">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="672ec-687">Cognitive Services</span></span>

* <span data-ttu-id="672ec-688">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="672ec-688">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-689">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-689">IoT</span></span>

* <span data-ttu-id="672ec-690">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-690">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-691">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-691">Monitor</span></span>

* <span data-ttu-id="672ec-692">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-692">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="672ec-693">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-693">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="672ec-694">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-694">Network</span></span>

* <span data-ttu-id="672ec-695">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-695">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-696">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-696">Resource</span></span>

* <span data-ttu-id="672ec-697">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-697">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-698">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-698">Storage</span></span>

* <span data-ttu-id="672ec-699">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-699">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-700">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-700">VM</span></span>

* <span data-ttu-id="672ec-701">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="672ec-701">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="672ec-702">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="672ec-702">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="672ec-703">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-703">Auguest 14, 2018</span></span>

<span data-ttu-id="672ec-704">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="672ec-704">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="672ec-705">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-705">Core</span></span>

* <span data-ttu-id="672ec-706">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-706">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="672ec-707">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-707">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="672ec-708">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="672ec-708">Telemetry</span></span>

* <span data-ttu-id="672ec-709">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="672ec-709">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-710">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-710">ACR</span></span>

* <span data-ttu-id="672ec-711">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-711">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="672ec-712">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-712">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-713">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-713">ACS</span></span>

* <span data-ttu-id="672ec-714">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-714">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="672ec-715">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="672ec-715">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="672ec-716">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="672ec-716">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="672ec-717">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="672ec-717">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="672ec-718">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="672ec-718">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="672ec-719">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-719">AppService</span></span>

* <span data-ttu-id="672ec-720">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="672ec-720">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="672ec-721">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-721">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="672ec-722">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-722">BatchAI</span></span>

* <span data-ttu-id="672ec-723">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="672ec-723">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="672ec-724">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-724">Container</span></span>

* <span data-ttu-id="672ec-725">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-725">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="672ec-726">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-726">IoT</span></span>

* <span data-ttu-id="672ec-727">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-727">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="672ec-728">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="672ec-728">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="672ec-729">Iot Central</span><span class="sxs-lookup"><span data-stu-id="672ec-729">Iot Central</span></span>

* <span data-ttu-id="672ec-730">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-730">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-731">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-731">KeyVault</span></span>


* <span data-ttu-id="672ec-732">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-732">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="672ec-733">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-733">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="672ec-734">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-734">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="672ec-735">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-735">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="672ec-736">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-736">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="672ec-737">Relay</span><span class="sxs-lookup"><span data-stu-id="672ec-737">Relay</span></span>

* <span data-ttu-id="672ec-738">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-738">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-739">Sql</span><span class="sxs-lookup"><span data-stu-id="672ec-739">Sql</span></span>

* <span data-ttu-id="672ec-740">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-740">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-741">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-741">Storage</span></span>

* <span data-ttu-id="672ec-742">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="672ec-742">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="672ec-743">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="672ec-743">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="672ec-744">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-744">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="672ec-745">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="672ec-745">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="672ec-746">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="672ec-746">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-747">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-747">VM</span></span>

* <span data-ttu-id="672ec-748">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-748">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="672ec-749">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-749">July 31, 2018</span></span>

<span data-ttu-id="672ec-750">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="672ec-750">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-751">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-751">ACR</span></span>

* <span data-ttu-id="672ec-752">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-752">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="672ec-753">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-753">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-754">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-754">ACS</span></span>

* <span data-ttu-id="672ec-755">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-755">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-756">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-756">Batch</span></span>

* <span data-ttu-id="672ec-757">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="672ec-757">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="672ec-758">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-758">Container</span></span>

* <span data-ttu-id="672ec-759">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-759">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="672ec-760">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-760">Network</span></span>

* <span data-ttu-id="672ec-761">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-761">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="672ec-762">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-762">Resource</span></span>

* <span data-ttu-id="672ec-763">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="672ec-763">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="672ec-764">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="672ec-764">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="672ec-765">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-765">Role</span></span>

* <span data-ttu-id="672ec-766">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-766">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="672ec-767">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="672ec-767">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="672ec-768">Suchen,</span><span class="sxs-lookup"><span data-stu-id="672ec-768">Search</span></span>

* <span data-ttu-id="672ec-769">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-769">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="672ec-770">Service Bus</span><span class="sxs-lookup"><span data-stu-id="672ec-770">Service Bus</span></span>

* <span data-ttu-id="672ec-771">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="672ec-771">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="672ec-772">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-772">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="672ec-773">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="672ec-773">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="672ec-774">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="672ec-774">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-775">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-775">Storage</span></span>

* <span data-ttu-id="672ec-776">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-776">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="672ec-777">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-777">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-778">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-778">VM</span></span>

* <span data-ttu-id="672ec-779">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-779">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="672ec-780">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-780">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="672ec-781">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-781">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="672ec-782">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-782">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="672ec-783">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-783">July 18, 2018</span></span>

<span data-ttu-id="672ec-784">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="672ec-784">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="672ec-785">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-785">Core</span></span>

* <span data-ttu-id="672ec-786">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-786">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="672ec-787">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-787">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="672ec-788">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="672ec-788">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-789">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-789">ACR</span></span>

* <span data-ttu-id="672ec-790">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-790">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="672ec-791">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-791">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="672ec-792">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-792">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="672ec-793">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-793">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-794">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-794">ACS</span></span>

* <span data-ttu-id="672ec-795">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="672ec-795">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-796">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-796">AppService</span></span>

* <span data-ttu-id="672ec-797">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-797">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-798">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-798">Batch</span></span>

* <span data-ttu-id="672ec-799">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="672ec-799">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="672ec-800">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-800">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="672ec-801">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-801">Batch AI</span></span>

* <span data-ttu-id="672ec-802">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-802">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="672ec-803">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-803">Container</span></span>

* <span data-ttu-id="672ec-804">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-804">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="672ec-805">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-805">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="672ec-806">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-806">Network</span></span>

* <span data-ttu-id="672ec-807">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-807">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="672ec-808">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-808">Added `network nic wait`</span></span>
* <span data-ttu-id="672ec-809">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-809">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="672ec-810">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="672ec-810">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="672ec-811">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-811">Resource</span></span>

* <span data-ttu-id="672ec-812">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-812">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="672ec-813">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-813">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="672ec-814">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-814">Added `deployment wait` command</span></span>
* <span data-ttu-id="672ec-815">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-815">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-816">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-816">SQL</span></span>

* <span data-ttu-id="672ec-817">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-817">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="672ec-818">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="672ec-818">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="672ec-819">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-819">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-820">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-820">Storage</span></span>

* <span data-ttu-id="672ec-821">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-821">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-822">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-822">VM</span></span>

* <span data-ttu-id="672ec-823">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-823">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="672ec-824">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-824">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="672ec-825">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-825">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="672ec-826">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-826">July 3, 2018</span></span>

<span data-ttu-id="672ec-827">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="672ec-827">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="672ec-828">AKS</span><span class="sxs-lookup"><span data-stu-id="672ec-828">AKS</span></span>

* <span data-ttu-id="672ec-829">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-829">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="672ec-830">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-830">July 3, 2018</span></span>

<span data-ttu-id="672ec-831">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="672ec-831">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="672ec-832">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-832">Core</span></span>

* <span data-ttu-id="672ec-833">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-833">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-834">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-834">ACR</span></span>

* <span data-ttu-id="672ec-835">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-835">Added polling build status</span></span>
* <span data-ttu-id="672ec-836">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-836">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="672ec-837">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-837">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-838">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-838">ACS</span></span>

* <span data-ttu-id="672ec-839">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="672ec-839">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="672ec-840">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="672ec-840">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="672ec-841">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-841">Updated options for `aks browse` command.</span></span> <span data-ttu-id="672ec-842">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-842">Added `--listen-port` support</span></span>
* <span data-ttu-id="672ec-843">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-843">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="672ec-844">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="672ec-844">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="672ec-845">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-845">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-846">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-846">AppService</span></span>

* <span data-ttu-id="672ec-847">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-847">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="672ec-848">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-848">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="672ec-849">Backup</span><span class="sxs-lookup"><span data-stu-id="672ec-849">Backup</span></span>

* <span data-ttu-id="672ec-850">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-850">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="672ec-851">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-851">BatchAI</span></span>

* <span data-ttu-id="672ec-852">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-852">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="672ec-853">Cloud</span><span class="sxs-lookup"><span data-stu-id="672ec-853">Cloud</span></span>

* <span data-ttu-id="672ec-854">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-854">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="672ec-855">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-855">Container</span></span>

* <span data-ttu-id="672ec-856">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-856">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="672ec-857">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-857">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="672ec-858">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-858">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-859">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-859">Extension</span></span>

* <span data-ttu-id="672ec-860">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-860">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="672ec-861">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-861">Network</span></span>

* <span data-ttu-id="672ec-862">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="672ec-862">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-863">Rdbms</span><span class="sxs-lookup"><span data-stu-id="672ec-863">Rdbms</span></span>

* <span data-ttu-id="672ec-864">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-864">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-865">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-865">Resource</span></span>

* <span data-ttu-id="672ec-866">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-866">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-867">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-867">VM</span></span>

* <span data-ttu-id="672ec-868">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-868">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="672ec-869">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-869">June 25, 2018</span></span>

<span data-ttu-id="672ec-870">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="672ec-870">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="672ec-871">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="672ec-871">CLI</span></span>

* <span data-ttu-id="672ec-872">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="672ec-872">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="672ec-873">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-873">June 19, 2018</span></span>

<span data-ttu-id="672ec-874">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="672ec-874">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="672ec-875">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-875">Core</span></span>

* <span data-ttu-id="672ec-876">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-876">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-877">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-877">ACR</span></span>

* <span data-ttu-id="672ec-878">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-878">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="672ec-879">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="672ec-879">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-880">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-880">ACS</span></span>

* <span data-ttu-id="672ec-881">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="672ec-881">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="672ec-882">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-882">Added `--update` support</span></span>
* <span data-ttu-id="672ec-883">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-883">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="672ec-884">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-884">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="672ec-885">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-885">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="672ec-886">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="672ec-886">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="672ec-887">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-887">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="672ec-888">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-888">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-889">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-889">AppService</span></span>

* <span data-ttu-id="672ec-890">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-890">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="672ec-891">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-891">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-892">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-892">Batch</span></span>

* <span data-ttu-id="672ec-893">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-893">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="672ec-894">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-894">Batch AI</span></span>

* <span data-ttu-id="672ec-895">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-895">Added support for workspaces.</span></span> <span data-ttu-id="672ec-896">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="672ec-896">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="672ec-897">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-897">Added support for experiments.</span></span> <span data-ttu-id="672ec-898">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="672ec-898">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="672ec-899">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-899">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="672ec-900">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-900">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="672ec-901">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="672ec-901">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="672ec-902">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-902">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="672ec-903">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-903">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="672ec-904">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-904">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="672ec-905">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-905">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="672ec-906">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="672ec-906">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="672ec-907">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-907">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="672ec-908">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="672ec-908">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="672ec-909">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-909">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="672ec-910">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="672ec-910">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="672ec-911">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-911">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="672ec-912">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="672ec-912">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="672ec-913">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-913">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="672ec-914">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-914">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="672ec-915">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-915">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="672ec-916">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-916">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="672ec-917">Karten</span><span class="sxs-lookup"><span data-stu-id="672ec-917">Maps</span></span>

* <span data-ttu-id="672ec-918">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="672ec-918">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="672ec-919">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-919">Network</span></span>

* <span data-ttu-id="672ec-920">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="672ec-920">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="672ec-921">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="672ec-921">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="672ec-922">#6502</span><span class="sxs-lookup"><span data-stu-id="672ec-922">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="672ec-923">Reservations</span><span class="sxs-lookup"><span data-stu-id="672ec-923">Reservations</span></span>

* <span data-ttu-id="672ec-924">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-924">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="672ec-925">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-925">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="672ec-926">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-926">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="672ec-927">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-927">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="672ec-928">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-928">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="672ec-929">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-929">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="672ec-930">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-930">Role</span></span>

* <span data-ttu-id="672ec-931">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-931">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-932">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-932">SQL</span></span>

* <span data-ttu-id="672ec-933">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="672ec-933">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-934">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-934">Storage</span></span>

* <span data-ttu-id="672ec-935">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-935">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-936">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-936">VM</span></span>

* <span data-ttu-id="672ec-937">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="672ec-937">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="672ec-938">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-938">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="672ec-939">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-939">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="672ec-940">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-940">June 13, 2018</span></span>

<span data-ttu-id="672ec-941">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="672ec-941">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="672ec-942">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-942">Core</span></span>

* <span data-ttu-id="672ec-943">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="672ec-943">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="672ec-944">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-944">June 13, 2018</span></span>

<span data-ttu-id="672ec-945">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="672ec-945">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="672ec-946">AKS</span><span class="sxs-lookup"><span data-stu-id="672ec-946">AKS</span></span>

* <span data-ttu-id="672ec-947">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-947">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="672ec-948">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-948">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="672ec-949">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-949">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="672ec-950">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-950">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="672ec-951">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-951">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-952">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-952">AppService</span></span>

* <span data-ttu-id="672ec-953">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-953">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="672ec-954">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-954">June 5, 2018</span></span>

<span data-ttu-id="672ec-955">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="672ec-955">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-956">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-956">Interactive</span></span>

* <span data-ttu-id="672ec-957">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-957">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="672ec-958">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-958">June 5, 2018</span></span>

<span data-ttu-id="672ec-959">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="672ec-959">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="672ec-960">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-960">Core</span></span>

* <span data-ttu-id="672ec-961">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-961">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="672ec-962">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="672ec-962">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-963">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-963">ACR</span></span>

* <span data-ttu-id="672ec-964">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-964">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="672ec-965">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-965">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="672ec-966">AKS</span><span class="sxs-lookup"><span data-stu-id="672ec-966">AKS</span></span>

* <span data-ttu-id="672ec-967">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="672ec-967">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-968">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-968">Batch</span></span>

* <span data-ttu-id="672ec-969">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="672ec-969">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-970">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-970">IOT</span></span>

* <span data-ttu-id="672ec-971">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-971">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="672ec-972">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-972">Network</span></span>

* <span data-ttu-id="672ec-973">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="672ec-973">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="672ec-974">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="672ec-974">Policy Insights</span></span>

* <span data-ttu-id="672ec-975">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-975">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="672ec-976">ARM</span><span class="sxs-lookup"><span data-stu-id="672ec-976">ARM</span></span>

* <span data-ttu-id="672ec-977">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-977">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-978">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-978">SQL</span></span>

* <span data-ttu-id="672ec-979">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-979">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="672ec-980">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-980">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="672ec-981">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-981">Storage</span></span>

* <span data-ttu-id="672ec-982">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="672ec-982">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-983">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-983">VM</span></span>

* <span data-ttu-id="672ec-984">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-984">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="672ec-985">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-985">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="672ec-986">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-986">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="672ec-987">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-987">May 22, 2018</span></span>

<span data-ttu-id="672ec-988">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="672ec-988">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="672ec-989">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-989">Core</span></span>

* <span data-ttu-id="672ec-990">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-990">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-991">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-991">ACS</span></span>

* <span data-ttu-id="672ec-992">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-992">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="672ec-993">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-993">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-994">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-994">AppService</span></span>

* <span data-ttu-id="672ec-995">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="672ec-995">Improved generic update commands</span></span>
* <span data-ttu-id="672ec-996">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-996">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="672ec-997">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-997">Container</span></span>

* <span data-ttu-id="672ec-998">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-998">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="672ec-999">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-999">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1000">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1000">Extension</span></span>

* <span data-ttu-id="672ec-1001">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="672ec-1001">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1002">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1002">Interactive</span></span>

* <span data-ttu-id="672ec-1003">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="672ec-1003">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="672ec-1004">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="672ec-1004">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-1005">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-1005">KeyVault</span></span>

* <span data-ttu-id="672ec-1006">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="672ec-1006">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1007">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1007">Network</span></span>

* <span data-ttu-id="672ec-1008">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="672ec-1008">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="672ec-1009">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="672ec-1009">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1010">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1010">SQL</span></span>

* <span data-ttu-id="672ec-1011">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="672ec-1011">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="672ec-1012">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1012">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="672ec-1013">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1013">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="672ec-1014">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="672ec-1014">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="672ec-1015">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="672ec-1015">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="672ec-1016">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1016">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="672ec-1017">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="672ec-1017">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="672ec-1018">`edition`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1018">`edition`.</span></span> <span data-ttu-id="672ec-1019">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="672ec-1019">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="672ec-1020">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1020">`elasticPoolName`.</span></span> <span data-ttu-id="672ec-1021">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="672ec-1021">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="672ec-1022">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="672ec-1022">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="672ec-1023">`edition`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1023">`edition`.</span></span> <span data-ttu-id="672ec-1024">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1024">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="672ec-1025">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1025">`dtu`.</span></span> <span data-ttu-id="672ec-1026">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1026">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="672ec-1027">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1027">`databaseDtuMin`.</span></span> <span data-ttu-id="672ec-1028">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1028">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="672ec-1029">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1029">`databaseDtuMax`.</span></span> <span data-ttu-id="672ec-1030">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1030">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="672ec-1031">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1031">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="672ec-1032">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1032">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1033">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1033">Storage</span></span>

* <span data-ttu-id="672ec-1034">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1034">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="672ec-1035">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1035">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1036">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1036">VM</span></span>

* <span data-ttu-id="672ec-1037">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1037">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="672ec-1038">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-1038">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="672ec-1039">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1039">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="672ec-1040">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1040">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="672ec-1041">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1041">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="672ec-1042">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1042">May 7, 2018</span></span>

<span data-ttu-id="672ec-1043">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="672ec-1043">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1044">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1044">Core</span></span>

* <span data-ttu-id="672ec-1045">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="672ec-1045">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="672ec-1046">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1046">Added limited support for positional arguments</span></span>
* <span data-ttu-id="672ec-1047">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-1047">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="672ec-1048">#5591</span><span class="sxs-lookup"><span data-stu-id="672ec-1048">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="672ec-1049">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1049">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="672ec-1050">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="672ec-1050">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="672ec-1051">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="672ec-1051">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="672ec-1052">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="672ec-1052">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="672ec-1053">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1053">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1054">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1054">ACR</span></span>

* <span data-ttu-id="672ec-1055">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1055">Added ACR Build commands</span></span>
* <span data-ttu-id="672ec-1056">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1056">Improved resource not found error messages</span></span>
* <span data-ttu-id="672ec-1057">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="672ec-1057">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="672ec-1058">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1058">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="672ec-1059">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1059">Improved repository commands error messages</span></span>
* <span data-ttu-id="672ec-1060">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1060">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1061">ACS</span></span>

* <span data-ttu-id="672ec-1062">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="672ec-1062">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="672ec-1063">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1063">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="672ec-1064">AMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1064">AMS</span></span>

* <span data-ttu-id="672ec-1065">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="672ec-1065">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1066">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1066">Appservice</span></span>

* <span data-ttu-id="672ec-1067">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="672ec-1067">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="672ec-1068">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1068">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="672ec-1069">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1069">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="672ec-1070">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1070">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="672ec-1071">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-1071">Batch AI</span></span>

* <span data-ttu-id="672ec-1072">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1072">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="672ec-1073">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="672ec-1073">Cognitive Services</span></span>

* <span data-ttu-id="672ec-1074">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="672ec-1074">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-1075">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-1075">Consumption</span></span>

* <span data-ttu-id="672ec-1076">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1076">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1077">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1077">Container</span></span>

* <span data-ttu-id="672ec-1078">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-1078">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="672ec-1079">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="672ec-1079">Cosmos DB</span></span>

* <span data-ttu-id="672ec-1080">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="672ec-1080">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="672ec-1081">DMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1081">DMS</span></span>

* <span data-ttu-id="672ec-1082">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1082">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1083">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1083">Extension</span></span>

* <span data-ttu-id="672ec-1084">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1084">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1085">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1085">Interactive</span></span>

* <span data-ttu-id="672ec-1086">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="672ec-1086">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="672ec-1087">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="672ec-1087">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="672ec-1088">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1088">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="672ec-1089">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1089">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="672ec-1090">Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-1090">Lab</span></span>

* <span data-ttu-id="672ec-1091">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1091">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1092">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1092">Network</span></span>

* <span data-ttu-id="672ec-1093">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="672ec-1093">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="672ec-1094">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1094">Profile</span></span>

* <span data-ttu-id="672ec-1095">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1095">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="672ec-1096">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="672ec-1096">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="672ec-1097">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1097">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="672ec-1098">Redis</span><span class="sxs-lookup"><span data-stu-id="672ec-1098">Redis</span></span>

* <span data-ttu-id="672ec-1099">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1099">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="672ec-1100">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1100">Deprecated `redis list-all`.</span></span> <span data-ttu-id="672ec-1101">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="672ec-1101">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="672ec-1102">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1102">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="672ec-1103">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1103">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="672ec-1104">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1104">Role</span></span>

* <span data-ttu-id="672ec-1105">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1105">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1106">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1106">Storage</span></span>

* <span data-ttu-id="672ec-1107">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="672ec-1107">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="672ec-1108">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="672ec-1108">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="672ec-1109">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="672ec-1109">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="672ec-1110">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="672ec-1110">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="672ec-1111">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="672ec-1111">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1112">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1112">VM</span></span>

* <span data-ttu-id="672ec-1113">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1113">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="672ec-1114">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1114">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="672ec-1115">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="672ec-1115">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="672ec-1116">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1116">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="672ec-1117">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="672ec-1117">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="672ec-1118">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1118">Added write accelerator support</span></span>
* <span data-ttu-id="672ec-1119">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1119">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="672ec-1120">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="672ec-1120">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="672ec-1121">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="672ec-1121">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="672ec-1122">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1122">April 10, 2018</span></span>

<span data-ttu-id="672ec-1123">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="672ec-1123">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1124">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1124">ACR</span></span>

* <span data-ttu-id="672ec-1125">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="672ec-1125">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1126">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1126">ACS</span></span>

* <span data-ttu-id="672ec-1127">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1127">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1128">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="672ec-1130">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1130">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="672ec-1131">Batch AI</span><span class="sxs-lookup"><span data-stu-id="672ec-1131">BatchAI</span></span>

* <span data-ttu-id="672ec-1132">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1132">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="672ec-1133">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="672ec-1133">Job level mounting</span></span>
  - <span data-ttu-id="672ec-1134">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="672ec-1134">Environment variables with secret values</span></span>
  - <span data-ttu-id="672ec-1135">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="672ec-1135">Performance counters settings</span></span>
  - <span data-ttu-id="672ec-1136">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="672ec-1136">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="672ec-1137">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="672ec-1137">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="672ec-1138">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="672ec-1138">Usage and limits reporting</span></span>
  - <span data-ttu-id="672ec-1139">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="672ec-1139">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="672ec-1140">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="672ec-1140">Support for custom images</span></span>
  - <span data-ttu-id="672ec-1141">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1141">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="672ec-1142">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="672ec-1142">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="672ec-1143">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="672ec-1143">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="672ec-1144">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="672ec-1144">National clouds are supported</span></span>
* <span data-ttu-id="672ec-1145">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1145">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="672ec-1146">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="672ec-1146">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="672ec-1147">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1147">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="672ec-1148">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="672ec-1148">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="672ec-1149">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="672ec-1149">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="672ec-1150">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="672ec-1150">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="672ec-1151">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="672ec-1151">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="672ec-1152">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1152">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="672ec-1153">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="672ec-1153">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="672ec-1154">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1154">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="672ec-1155">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="672ec-1155">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="672ec-1156">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1156">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="672ec-1157">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="672ec-1157">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="672ec-1158">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="672ec-1158">Billing</span></span>

* <span data-ttu-id="672ec-1159">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1159">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-1160">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-1160">Consumption</span></span>

* <span data-ttu-id="672ec-1161">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1161">Added `marketplace` commands</span></span>
* <span data-ttu-id="672ec-1162">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1162">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="672ec-1163">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1163">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="672ec-1164">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1164">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="672ec-1165">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1165">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="672ec-1166">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1166">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1167">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1167">Container</span></span>

* <span data-ttu-id="672ec-1168">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1168">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="672ec-1169">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-1169">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1170">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1170">Extension</span></span>

* <span data-ttu-id="672ec-1171">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1171">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1172">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1172">Interactive</span></span>

* <span data-ttu-id="672ec-1173">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="672ec-1173">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="672ec-1174">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1174">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="672ec-1175">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1175">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1176">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1176">Network</span></span>

* <span data-ttu-id="672ec-1177">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-1177">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="672ec-1178">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1178">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="672ec-1179">#4910</span><span class="sxs-lookup"><span data-stu-id="672ec-1179">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="672ec-1180">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1180">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="672ec-1181">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1181">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="672ec-1182">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1182">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="672ec-1183">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1183">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="672ec-1184">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1184">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1185">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1185">Profile</span></span>

* <span data-ttu-id="672ec-1186">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1186">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="672ec-1187">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1187">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-1188">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1188">RDBMS</span></span>

* <span data-ttu-id="672ec-1189">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1189">Added `georestore` command</span></span>
* <span data-ttu-id="672ec-1190">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1190">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1191">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1191">Resource</span></span>

* <span data-ttu-id="672ec-1192">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1192">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="672ec-1193">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1193">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1194">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1194">SQL</span></span>

* <span data-ttu-id="672ec-1195">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1195">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1196">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1196">Storage</span></span>

* <span data-ttu-id="672ec-1197">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1197">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1198">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1198">VM</span></span>

* <span data-ttu-id="672ec-1199">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1199">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="672ec-1200">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1200">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="672ec-1202">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1202">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="672ec-1203">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="672ec-1203">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="672ec-1204">#5718</span><span class="sxs-lookup"><span data-stu-id="672ec-1204">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="672ec-1205">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="672ec-1205">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="672ec-1206">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1206">March 27, 2018</span></span>

<span data-ttu-id="672ec-1207">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="672ec-1207">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1208">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1208">Core</span></span>

* <span data-ttu-id="672ec-1209">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="672ec-1209">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1210">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1210">ACS</span></span>

* <span data-ttu-id="672ec-1211">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="672ec-1211">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1212">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1212">Appservice</span></span>

* <span data-ttu-id="672ec-1213">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1213">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="672ec-1214">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1214">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="672ec-1215">Backup</span><span class="sxs-lookup"><span data-stu-id="672ec-1215">Backup</span></span>

* <span data-ttu-id="672ec-1216">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1216">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="672ec-1217">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="672ec-1217">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="672ec-1218">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="672ec-1218">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="672ec-1219">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="672ec-1219">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1220">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1220">Container</span></span>

* <span data-ttu-id="672ec-1221">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1221">Added `container exec` command.</span></span> <span data-ttu-id="672ec-1222">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="672ec-1222">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="672ec-1223">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="672ec-1223">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1224">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1224">Extension</span></span>

* <span data-ttu-id="672ec-1225">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="672ec-1225">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="672ec-1226">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-1226">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="672ec-1227">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-1227">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1228">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1228">Interactive</span></span>

* <span data-ttu-id="672ec-1229">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-1229">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="672ec-1230">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1230">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="672ec-1231">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="672ec-1231">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="672ec-1232">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="672ec-1232">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="672ec-1233">Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-1233">Lab</span></span>

* <span data-ttu-id="672ec-1234">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1234">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1235">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1235">Monitor</span></span>

* <span data-ttu-id="672ec-1236">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="672ec-1236">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="672ec-1237">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="672ec-1237">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="672ec-1238">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="672ec-1238">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1239">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1239">Network</span></span>

* <span data-ttu-id="672ec-1240">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1240">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1241">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1241">Profile</span></span>

* <span data-ttu-id="672ec-1242">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1242">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-1243">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1243">RDBMS</span></span>

* <span data-ttu-id="672ec-1244">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1244">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1245">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1245">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="672ec-1247">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1247">Role</span></span>

* <span data-ttu-id="672ec-1248">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1248">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="672ec-1249">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="672ec-1249">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="672ec-1250">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1250">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="672ec-1251">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1251">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="672ec-1252">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1252">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1253">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1253">Storage</span></span>

* <span data-ttu-id="672ec-1254">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1254">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="672ec-1255">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="672ec-1255">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1256">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1256">VM</span></span>

* <span data-ttu-id="672ec-1257">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1257">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="672ec-1258">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1258">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="672ec-1259">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="672ec-1259">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="672ec-1260">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="672ec-1260">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="672ec-1261">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1261">March 13, 2018</span></span>

<span data-ttu-id="672ec-1262">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="672ec-1262">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1263">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1263">ACR</span></span>

* <span data-ttu-id="672ec-1264">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1264">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="672ec-1265">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1265">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="672ec-1266">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1266">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1267">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1267">ACS</span></span>

* <span data-ttu-id="672ec-1268">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1268">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="672ec-1269">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1269">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="672ec-1270">Advisor</span><span class="sxs-lookup"><span data-stu-id="672ec-1270">Advisor</span></span>

* <span data-ttu-id="672ec-1271">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1271">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="672ec-1272">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1272">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="672ec-1273">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1273">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="672ec-1274">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1274">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="672ec-1275">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1275">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1276">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1276">Appservice</span></span>

* <span data-ttu-id="672ec-1277">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1277">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="672ec-1278">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1278">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="672ec-1279">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="672ec-1279">Eventhubs</span></span>

* <span data-ttu-id="672ec-1280">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1280">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1281">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1281">Extension</span></span>

* <span data-ttu-id="672ec-1282">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="672ec-1282">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1283">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1283">Interactive</span></span>

* <span data-ttu-id="672ec-1284">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="672ec-1284">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="672ec-1285">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="672ec-1285">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="672ec-1286">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="672ec-1286">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="672ec-1287">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1287">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1288">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1288">Monitor</span></span>

* <span data-ttu-id="672ec-1289">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1289">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="672ec-1290">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1290">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="672ec-1291">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1291">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="672ec-1292">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1292">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1293">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1293">Network</span></span>

* <span data-ttu-id="672ec-1294">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1294">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="672ec-1295">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="672ec-1295">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="672ec-1296">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1296">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="672ec-1297">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1297">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1298">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1298">Profile</span></span>

* <span data-ttu-id="672ec-1299">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1299">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="672ec-1300">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1300">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-1301">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1301">RDBMS</span></span>

* <span data-ttu-id="672ec-1302">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1302">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="672ec-1303">Service Bus</span><span class="sxs-lookup"><span data-stu-id="672ec-1303">Service Bus</span></span>

* <span data-ttu-id="672ec-1304">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1304">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1305">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1305">Storage</span></span>

* <span data-ttu-id="672ec-1306">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="672ec-1306">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="672ec-1307">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="672ec-1307">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1308">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1308">VM</span></span>

* <span data-ttu-id="672ec-1309">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="672ec-1309">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="672ec-1310">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1310">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="672ec-1311">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1311">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="672ec-1312">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1312">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="672ec-1313">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1313">February 27, 2018</span></span>

<span data-ttu-id="672ec-1314">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="672ec-1314">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1315">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1315">Core</span></span>

* <span data-ttu-id="672ec-1316">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="672ec-1316">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="672ec-1317">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1317">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="672ec-1318">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1318">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1319">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1319">ACS</span></span>

* <span data-ttu-id="672ec-1320">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1320">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="672ec-1321">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="672ec-1321">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="672ec-1322">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1322">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="672ec-1323">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1323">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1324">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1324">Appservice</span></span>

* <span data-ttu-id="672ec-1325">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="672ec-1325">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="672ec-1326">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="672ec-1326">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="672ec-1327">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="672ec-1327">Cognitive Services</span></span>

* <span data-ttu-id="672ec-1328">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1328">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-1329">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-1329">Consumption</span></span>

* <span data-ttu-id="672ec-1330">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1330">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="672ec-1331">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1331">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1332">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1332">Container</span></span>

* <span data-ttu-id="672ec-1333">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="672ec-1333">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1334">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1334">Network</span></span>

* <span data-ttu-id="672ec-1335">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="672ec-1335">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1336">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1336">Resource</span></span>

* <span data-ttu-id="672ec-1337">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="672ec-1337">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="672ec-1338">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1338">Role</span></span>

* <span data-ttu-id="672ec-1339">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1339">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1340">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1340">SQL</span></span>

* <span data-ttu-id="672ec-1341">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="672ec-1341">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1342">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1342">Storage</span></span>

* <span data-ttu-id="672ec-1343">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-1343">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1344">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1344">VM</span></span>

* <span data-ttu-id="672ec-1345">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1345">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="672ec-1346">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1346">February 13, 2018</span></span>

<span data-ttu-id="672ec-1347">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="672ec-1347">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1348">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1348">Core</span></span>

* <span data-ttu-id="672ec-1349">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1349">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1350">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1350">ACS</span></span>

* <span data-ttu-id="672ec-1351">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1351">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="672ec-1352">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1352">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="672ec-1353">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1353">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="672ec-1354">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1354">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="672ec-1355">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1355">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="672ec-1356">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1356">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="672ec-1357">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="672ec-1357">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="672ec-1358">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="672ec-1358">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1359">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1359">Appservice</span></span>

* <span data-ttu-id="672ec-1360">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="672ec-1360">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="672ec-1361">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1361">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="672ec-1362">CDN</span><span class="sxs-lookup"><span data-stu-id="672ec-1362">CDN</span></span>

* <span data-ttu-id="672ec-1363">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1363">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1364">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1364">Container</span></span>

* <span data-ttu-id="672ec-1365">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1365">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="672ec-1366">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1366">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-1367">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-1367">CosmosDB</span></span>

* <span data-ttu-id="672ec-1368">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1368">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1369">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1369">Extension</span></span>

* <span data-ttu-id="672ec-1370">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1370">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="672ec-1371">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1371">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="672ec-1372">Feedback</span><span class="sxs-lookup"><span data-stu-id="672ec-1372">Feedback</span></span>

* <span data-ttu-id="672ec-1373">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1373">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1374">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1374">Interactive</span></span>

* <span data-ttu-id="672ec-1375">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1375">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="672ec-1376">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1376">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-1377">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-1377">IoT</span></span>

* <span data-ttu-id="672ec-1378">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="672ec-1378">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="672ec-1379">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="672ec-1379">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="672ec-1380">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1380">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="672ec-1381">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1381">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1382">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1382">Monitor</span></span>

* <span data-ttu-id="672ec-1383">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1383">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1384">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1384">Network</span></span>

* <span data-ttu-id="672ec-1385">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="672ec-1385">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="672ec-1386">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1386">Profile</span></span>

* <span data-ttu-id="672ec-1387">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="672ec-1387">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1388">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1388">Resource</span></span>

* <span data-ttu-id="672ec-1389">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1389">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="672ec-1390">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1390">Role</span></span>

* <span data-ttu-id="672ec-1391">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1391">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1392">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1392">SQL</span></span>

* <span data-ttu-id="672ec-1393">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1393">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="672ec-1394">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1394">Added `sql db rename`</span></span>
* <span data-ttu-id="672ec-1395">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1395">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1396">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1396">Storage</span></span>

* <span data-ttu-id="672ec-1397">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1397">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1398">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1398">VM</span></span>

* <span data-ttu-id="672ec-1399">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1399">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="672ec-1400">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1400">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="672ec-1401">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="672ec-1401">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="672ec-1402">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1402">January 31, 2018</span></span>

<span data-ttu-id="672ec-1403">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="672ec-1403">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1404">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1404">Core</span></span>

* <span data-ttu-id="672ec-1405">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1405">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="672ec-1406">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1406">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="672ec-1407">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="672ec-1407">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="672ec-1408">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="672ec-1408">Use `--verbose` to see</span></span>
* <span data-ttu-id="672ec-1409">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1409">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1410">ACS</span></span>

* <span data-ttu-id="672ec-1411">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="672ec-1411">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="672ec-1412">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1412">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1413">Appservice</span></span>

* <span data-ttu-id="672ec-1414">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="672ec-1414">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="672ec-1415">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1415">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="672ec-1416">CDN</span><span class="sxs-lookup"><span data-stu-id="672ec-1416">CDN</span></span>

* <span data-ttu-id="672ec-1417">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1417">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-1418">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-1418">CosmosDB</span></span>

* <span data-ttu-id="672ec-1419">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1419">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1420">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1420">Interactive</span></span>

* <span data-ttu-id="672ec-1421">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1421">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1422">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1422">Network</span></span>

* <span data-ttu-id="672ec-1423">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1423">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="672ec-1424">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="672ec-1424">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="672ec-1425">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1425">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="672ec-1426">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1426">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="672ec-1427">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1427">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="672ec-1428">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="672ec-1428">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="672ec-1429">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1429">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="672ec-1430">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1430">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="672ec-1431">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1431">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="672ec-1432">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="672ec-1432">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1433">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1433">Profile</span></span>

* <span data-ttu-id="672ec-1434">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1434">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1435">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1435">Resource</span></span>

* <span data-ttu-id="672ec-1436">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="672ec-1436">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1437">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1437">Storage</span></span>

* <span data-ttu-id="672ec-1438">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1438">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="672ec-1439">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1439">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="672ec-1440">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="672ec-1440">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="672ec-1441">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1441">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="672ec-1442">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="672ec-1442">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1443">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1443">VM</span></span>

* <span data-ttu-id="672ec-1444">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1444">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="672ec-1445">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="672ec-1445">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="672ec-1446">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1446">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="672ec-1447">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1447">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="672ec-1448">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="672ec-1448">January 17, 2018</span></span>

<span data-ttu-id="672ec-1449">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="672ec-1449">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1450">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1450">ACR</span></span>

* <span data-ttu-id="672ec-1451">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1451">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="672ec-1452">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="672ec-1452">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1453">ACS</span></span>

* <span data-ttu-id="672ec-1454">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1454">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="672ec-1455">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1455">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1456">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1456">Appservice</span></span>

* <span data-ttu-id="672ec-1457">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="672ec-1457">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="672ec-1458">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1458">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="672ec-1459">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1459">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="672ec-1460">Backup</span><span class="sxs-lookup"><span data-stu-id="672ec-1460">Backup</span></span>

* <span data-ttu-id="672ec-1461">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="672ec-1461">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="672ec-1462">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1462">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="672ec-1463">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="672ec-1463">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="672ec-1464">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="672ec-1464">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="672ec-1465">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="672ec-1465">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-1466">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-1466">Batch</span></span>

* <span data-ttu-id="672ec-1467">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="672ec-1467">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="672ec-1468">Cloud</span><span class="sxs-lookup"><span data-stu-id="672ec-1468">Cloud</span></span>

* <span data-ttu-id="672ec-1469">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1469">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-1470">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-1470">Consumption</span></span>

* <span data-ttu-id="672ec-1471">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="672ec-1471">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="672ec-1472">Event Grid</span><span class="sxs-lookup"><span data-stu-id="672ec-1472">Event Grid</span></span>

* <span data-ttu-id="672ec-1473">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-1473">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="672ec-1474">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-1474">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="672ec-1475">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1475">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="672ec-1476">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1476">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="672ec-1477">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1477">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="672ec-1478">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1478">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="672ec-1479">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1479">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="672ec-1480">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1480">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1481">Interactive</span><span class="sxs-lookup"><span data-stu-id="672ec-1481">Interactive</span></span>

* <span data-ttu-id="672ec-1482">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-1482">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="672ec-1483">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1483">Fixed errors on startup</span></span>
* <span data-ttu-id="672ec-1484">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="672ec-1484">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-1485">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-1485">IoT</span></span>

* <span data-ttu-id="672ec-1486">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1486">Added support for device provisioning service</span></span>
* <span data-ttu-id="672ec-1487">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1487">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="672ec-1488">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="672ec-1488">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1489">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1489">Monitor</span></span>

* <span data-ttu-id="672ec-1490">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1490">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="672ec-1491">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="672ec-1491">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="672ec-1492">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1492">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1493">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1493">Network</span></span>

* <span data-ttu-id="672ec-1494">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="672ec-1494">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="672ec-1495">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1495">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1496">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1496">Profile</span></span>

* <span data-ttu-id="672ec-1497">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1497">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="672ec-1498">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1498">Role</span></span>

* <span data-ttu-id="672ec-1499">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="672ec-1499">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="672ec-1500">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="672ec-1500">Service Fabric</span></span>

* <span data-ttu-id="672ec-1501">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1501">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="672ec-1502">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1502">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1503">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1503">VM</span></span>

* <span data-ttu-id="672ec-1504">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="672ec-1504">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="672ec-1505">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1505">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="672ec-1506">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="672ec-1506">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="672ec-1507">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1507">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="672ec-1508">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1508">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="672ec-1509">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1509">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="672ec-1510">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1510">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="672ec-1511">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1511">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="672ec-1512">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1512">December 19, 2017</span></span>

<span data-ttu-id="672ec-1513">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="672ec-1513">Version 2.0.23</span></span>

* <span data-ttu-id="672ec-1514">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1514">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1515">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1515">Container</span></span>

* <span data-ttu-id="672ec-1516">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1516">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1517">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1517">Network</span></span>

* <span data-ttu-id="672ec-1518">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1518">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="672ec-1519">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1519">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1520">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1520">Storage</span></span>

* <span data-ttu-id="672ec-1521">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1521">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1522">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1522">VM</span></span>

* <span data-ttu-id="672ec-1523">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1523">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="672ec-1524">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1524">December 5, 2017</span></span>

<span data-ttu-id="672ec-1525">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="672ec-1525">Version 2.0.22</span></span>

* <span data-ttu-id="672ec-1526">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1526">Removed `az component` commands.</span></span> <span data-ttu-id="672ec-1527">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1527">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1528">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1528">Core</span></span>
* <span data-ttu-id="672ec-1529">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="672ec-1529">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="672ec-1530">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1530">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1531">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1531">ACS</span></span>

* <span data-ttu-id="672ec-1532">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1532">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="672ec-1533">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="672ec-1533">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="672ec-1534">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="672ec-1534">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="672ec-1535">Advisor</span><span class="sxs-lookup"><span data-stu-id="672ec-1535">Advisor</span></span>

* <span data-ttu-id="672ec-1536">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1536">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1537">Appservice</span></span>

* <span data-ttu-id="672ec-1538">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="672ec-1538">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="672ec-1539">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="672ec-1539">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="672ec-1540">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1540">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="672ec-1541">Nutzung</span><span class="sxs-lookup"><span data-stu-id="672ec-1541">Consumption</span></span>

* <span data-ttu-id="672ec-1542">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1542">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1543">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1543">Container</span></span>

* <span data-ttu-id="672ec-1544">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="672ec-1544">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1545">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1545">Monitor</span></span>

* <span data-ttu-id="672ec-1546">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1546">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1547">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1547">Resource</span></span>

* <span data-ttu-id="672ec-1548">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1548">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="672ec-1549">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-1549">Role</span></span>

* <span data-ttu-id="672ec-1550">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1550">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="672ec-1551">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1551">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="672ec-1552">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="672ec-1552">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1553">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1553">SQL</span></span>

* <span data-ttu-id="672ec-1554">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1554">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="672ec-1555">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1555">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1556">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1556">VM</span></span>

* <span data-ttu-id="672ec-1557">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1557">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="672ec-1558">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1558">November 14, 2017</span></span>

<span data-ttu-id="672ec-1559">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="672ec-1559">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1560">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1560">ACR</span></span>

* <span data-ttu-id="672ec-1561">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1561">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="672ec-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1562">ACS</span></span>

* <span data-ttu-id="672ec-1563">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1563">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="672ec-1564">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="672ec-1564">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="672ec-1565">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="672ec-1565">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="672ec-1566">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1566">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="672ec-1567">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1567">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1568">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1568">Appservice</span></span>

* <span data-ttu-id="672ec-1569">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1569">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="672ec-1570">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1570">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="672ec-1571">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1571">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="672ec-1572">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1572">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="672ec-1573">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1573">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="672ec-1574">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="672ec-1574">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-1575">Batch</span></span>

* <span data-ttu-id="672ec-1576">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="672ec-1576">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="672ec-1577">BatchAI</span><span class="sxs-lookup"><span data-stu-id="672ec-1577">Batchai</span></span>

* <span data-ttu-id="672ec-1578">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1578">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="672ec-1579">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1579">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="672ec-1580">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1580">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="672ec-1581">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1581">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="672ec-1582">Cloud</span><span class="sxs-lookup"><span data-stu-id="672ec-1582">Cloud</span></span>

* <span data-ttu-id="672ec-1583">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="672ec-1583">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1584">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1584">Container</span></span>

* <span data-ttu-id="672ec-1585">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1585">Added support to open multiple ports</span></span>
* <span data-ttu-id="672ec-1586">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1586">Added container group restart policy</span></span>
* <span data-ttu-id="672ec-1587">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1587">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="672ec-1588">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1588">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="672ec-1589">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="672ec-1589">Data Lake Analytics</span></span>

* <span data-ttu-id="672ec-1590">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="672ec-1590">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="672ec-1591">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="672ec-1591">Data Lake Store</span></span>

* <span data-ttu-id="672ec-1592">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="672ec-1592">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1593">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1593">Extension</span></span>

* <span data-ttu-id="672ec-1594">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1594">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="672ec-1595">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="672ec-1595">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-1596">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-1596">IoT</span></span>

* <span data-ttu-id="672ec-1597">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1597">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1598">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1598">Monitor</span></span>

* <span data-ttu-id="672ec-1599">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1599">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1600">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1600">Network</span></span>

* <span data-ttu-id="672ec-1601">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1601">Added support for CAA DNS records</span></span>
* <span data-ttu-id="672ec-1602">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="672ec-1602">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="672ec-1603">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="672ec-1603">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="672ec-1604">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1604">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="672ec-1605">Reservations</span><span class="sxs-lookup"><span data-stu-id="672ec-1605">Reservations</span></span>

* <span data-ttu-id="672ec-1606">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="672ec-1606">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1607">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1607">Resource</span></span>

* <span data-ttu-id="672ec-1608">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1608">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1609">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1609">SQL</span></span>

* <span data-ttu-id="672ec-1610">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1610">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1611">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1611">Storage</span></span>

* <span data-ttu-id="672ec-1612">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1612">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="672ec-1613">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="672ec-1613">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="672ec-1614">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="672ec-1614">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="672ec-1615">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1615">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="672ec-1616">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1616">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="672ec-1617">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1617">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="672ec-1618">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1618">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1619">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1619">VM</span></span>

* <span data-ttu-id="672ec-1620">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="672ec-1620">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="672ec-1621">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1621">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="672ec-1622">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="672ec-1622">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="672ec-1623">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1623">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="672ec-1624">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1624">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="672ec-1625">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1625">October 24, 2017</span></span>

<span data-ttu-id="672ec-1626">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="672ec-1626">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1627">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1627">Core</span></span>

* <span data-ttu-id="672ec-1628">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="672ec-1628">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1629">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1629">ACR</span></span>

* <span data-ttu-id="672ec-1630">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1630">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="672ec-1631">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="672ec-1631">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="672ec-1632">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1632">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1633">ACS</span></span>

* <span data-ttu-id="672ec-1634">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1634">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="672ec-1635">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1635">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1636">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1636">Appservice</span></span>

* <span data-ttu-id="672ec-1637">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="672ec-1637">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="672ec-1638">Komponente</span><span class="sxs-lookup"><span data-stu-id="672ec-1638">Component</span></span>

* <span data-ttu-id="672ec-1639">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1639">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1640">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1640">Monitor</span></span>

* <span data-ttu-id="672ec-1641">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1641">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1642">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1642">Resource</span></span>

* <span data-ttu-id="672ec-1643">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1643">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="672ec-1644">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="672ec-1644">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1645">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1645">VM</span></span>

* <span data-ttu-id="672ec-1646">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1646">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="672ec-1647">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1647">October 9, 2017</span></span>

<span data-ttu-id="672ec-1648">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="672ec-1648">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1649">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1649">Core</span></span>

* <span data-ttu-id="672ec-1650">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1650">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1651">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1651">Appservice</span></span>

* <span data-ttu-id="672ec-1652">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1652">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-1653">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-1653">Batch</span></span>

* <span data-ttu-id="672ec-1654">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="672ec-1654">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="672ec-1655">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1655">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="672ec-1656">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1656">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="672ec-1657">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1657">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="672ec-1658">BatchAI</span><span class="sxs-lookup"><span data-stu-id="672ec-1658">Batchai</span></span>

* <span data-ttu-id="672ec-1659">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-1659">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-1660">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-1660">Keyvault</span></span>

* <span data-ttu-id="672ec-1661">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="672ec-1661">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="672ec-1662">(#4448)</span><span class="sxs-lookup"><span data-stu-id="672ec-1662">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="672ec-1663">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1663">Network</span></span>

* <span data-ttu-id="672ec-1664">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="672ec-1664">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="672ec-1665">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1665">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1666">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1666">Resource</span></span>

* <span data-ttu-id="672ec-1667">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1667">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="672ec-1668">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1668">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="672ec-1669">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1669">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="672ec-1670">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1670">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1671">Sql</span><span class="sxs-lookup"><span data-stu-id="672ec-1671">Sql</span></span>

* <span data-ttu-id="672ec-1672">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1672">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="672ec-1673">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1673">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="672ec-1674">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1674">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1675">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1675">Storage</span></span>

* <span data-ttu-id="672ec-1676">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1676">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1677">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1677">Vm</span></span>

* <span data-ttu-id="672ec-1678">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="672ec-1678">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="672ec-1679">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1679">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="672ec-1680">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1680">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="672ec-1681">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1681">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="672ec-1682">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1682">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="672ec-1683">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1683">September 22, 2017</span></span>

<span data-ttu-id="672ec-1684">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="672ec-1684">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1685">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1685">Resource</span></span>

* <span data-ttu-id="672ec-1686">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1686">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="672ec-1687">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1687">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="672ec-1688">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1688">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="672ec-1689">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="672ec-1689">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1690">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1690">Network</span></span>

* <span data-ttu-id="672ec-1691">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1691">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="672ec-1692">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1692">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="672ec-1693">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1693">Added `asg` application security group commands</span></span>
* <span data-ttu-id="672ec-1694">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1694">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="672ec-1695">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1695">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="672ec-1696">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1696">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="672ec-1697">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1697">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1698">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1698">Storage</span></span>

* <span data-ttu-id="672ec-1699">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="672ec-1699">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="672ec-1700">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="672ec-1700">Eventgrid</span></span>

* <span data-ttu-id="672ec-1701">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1701">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1702">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1702">SQL</span></span>

* <span data-ttu-id="672ec-1703">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="672ec-1703">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="672ec-1704">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="672ec-1704">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="672ec-1705">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1705">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-1706">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-1706">Keyvault</span></span>

* <span data-ttu-id="672ec-1707">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1707">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1708">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1708">VM</span></span>

* <span data-ttu-id="672ec-1709">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1709">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="672ec-1710">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="672ec-1710">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="672ec-1711">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1711">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="672ec-1712">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1712">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="672ec-1713">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1713">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="672ec-1714">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1714">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1715">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1715">ACS</span></span>

* <span data-ttu-id="672ec-1716">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1716">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1717">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1717">Appservice</span></span>

* <span data-ttu-id="672ec-1718">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="672ec-1718">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="672ec-1719">Backup</span><span class="sxs-lookup"><span data-stu-id="672ec-1719">Backup</span></span>

* <span data-ttu-id="672ec-1720">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="672ec-1720">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="672ec-1721">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1721">September 11, 2017</span></span>

<span data-ttu-id="672ec-1722">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="672ec-1722">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="672ec-1723">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1723">Core</span></span>

* <span data-ttu-id="672ec-1724">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="672ec-1724">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="672ec-1725">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="672ec-1725">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1726">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1726">Acs</span></span>

* <span data-ttu-id="672ec-1727">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1727">Added `acs list-locations` command</span></span>
* <span data-ttu-id="672ec-1728">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="672ec-1728">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1729">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1729">Appservice</span></span>

* <span data-ttu-id="672ec-1730">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="672ec-1730">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="672ec-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="672ec-1731">CDN</span></span>

* <span data-ttu-id="672ec-1732">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="672ec-1732">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="672ec-1733">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="672ec-1733">Extension</span></span>

* <span data-ttu-id="672ec-1734">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1734">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-1735">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-1735">Keyvault</span></span>

* <span data-ttu-id="672ec-1736">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="672ec-1736">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1737">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1737">Network</span></span>

* <span data-ttu-id="672ec-1738">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1738">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="672ec-1739">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1739">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="672ec-1740">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1740">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="672ec-1741">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1741">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="672ec-1742">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1742">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1743">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1743">Resource</span></span>

* <span data-ttu-id="672ec-1744">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="672ec-1744">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="672ec-1745">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="672ec-1745">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="672ec-1746">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="672ec-1746">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="672ec-1747">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1747">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-1748">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-1748">SQL</span></span>

* <span data-ttu-id="672ec-1749">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1749">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1750">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1750">VM</span></span>

* <span data-ttu-id="672ec-1751">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1751">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="672ec-1752">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="672ec-1752">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="672ec-1753">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1753">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="672ec-1754">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="672ec-1754">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="672ec-1755">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="672ec-1755">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="672ec-1756">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1756">August 31, 2017</span></span>

<span data-ttu-id="672ec-1757">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="672ec-1757">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-1758">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-1758">Keyvault</span></span>

* <span data-ttu-id="672ec-1759">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="672ec-1759">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="672ec-1760">Sf</span><span class="sxs-lookup"><span data-stu-id="672ec-1760">Sf</span></span>

* <span data-ttu-id="672ec-1761">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1761">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1762">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1762">Storage</span></span>

* <span data-ttu-id="672ec-1763">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="672ec-1763">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="672ec-1764">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="672ec-1764">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="672ec-1765">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1765">August 28, 2017</span></span>

<span data-ttu-id="672ec-1766">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="672ec-1766">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="672ec-1767">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="672ec-1767">CLI</span></span>

* <span data-ttu-id="672ec-1768">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1768">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1769">ACS</span></span>

* <span data-ttu-id="672ec-1770">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1770">Corrected preview regions</span></span>
* <span data-ttu-id="672ec-1771">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1771">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="672ec-1772">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1772">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1773">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1773">Appservice</span></span>

* <span data-ttu-id="672ec-1774">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1774">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="672ec-1775">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1775">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="672ec-1776">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1776">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="672ec-1777">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="672ec-1777">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="672ec-1778">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="672ec-1778">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-1779">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-1779">IoT</span></span>

* <span data-ttu-id="672ec-1780">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="672ec-1780">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1781">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1781">Network</span></span>

* <span data-ttu-id="672ec-1782">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1782">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="672ec-1783">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1783">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="672ec-1784">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1784">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="672ec-1785">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1785">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="672ec-1786">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1786">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1787">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1787">Profile</span></span>

* <span data-ttu-id="672ec-1788">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1788">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="672ec-1789">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="672ec-1789">Service Fabric</span></span>

* <span data-ttu-id="672ec-1790">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="672ec-1790">Preview release</span></span>
* <span data-ttu-id="672ec-1791">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1791">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="672ec-1792">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1792">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="672ec-1793">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1793">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1794">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1794">Storage</span></span>

* <span data-ttu-id="672ec-1795">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-1795">Enabled setting blob tier</span></span>
* <span data-ttu-id="672ec-1796">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1796">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="672ec-1797">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1797">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="672ec-1798">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-1798">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="672ec-1799">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1799">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="672ec-1800">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="672ec-1800">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1801">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1801">VM</span></span>

* <span data-ttu-id="672ec-1802">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1802">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="672ec-1803">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-1803">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="672ec-1804">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1804">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="672ec-1805">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="672ec-1805">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="672ec-1806">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1806">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="672ec-1807">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-1807">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="672ec-1808">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1808">August 15, 2017</span></span>

<span data-ttu-id="672ec-1809">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="672ec-1809">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1810">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1810">ACS</span></span>

* <span data-ttu-id="672ec-1811">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1811">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1812">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1812">Appservice</span></span>

* <span data-ttu-id="672ec-1813">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1813">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="672ec-1814">Event Grid</span><span class="sxs-lookup"><span data-stu-id="672ec-1814">Event Grid</span></span>

* <span data-ttu-id="672ec-1815">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1815">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="672ec-1816">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1816">August 11, 2017</span></span>

<span data-ttu-id="672ec-1817">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="672ec-1817">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1818">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1818">ACS</span></span>

* <span data-ttu-id="672ec-1819">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1819">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-1820">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-1820">Batch</span></span>

* <span data-ttu-id="672ec-1821">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1821">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="672ec-1822">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1822">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="672ec-1823">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1823">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="672ec-1824">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="672ec-1824">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="672ec-1825">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="672ec-1825">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="672ec-1826">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1826">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="672ec-1827">Komponente</span><span class="sxs-lookup"><span data-stu-id="672ec-1827">Component</span></span>

* <span data-ttu-id="672ec-1828">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1828">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="672ec-1829">Container</span><span class="sxs-lookup"><span data-stu-id="672ec-1829">Container</span></span>

* <span data-ttu-id="672ec-1830">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="672ec-1830">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="672ec-1831">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="672ec-1831">Data Lake Store</span></span>

* <span data-ttu-id="672ec-1832">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-1832">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="672ec-1833">Event Grid</span><span class="sxs-lookup"><span data-stu-id="672ec-1833">Event Grid</span></span>

* <span data-ttu-id="672ec-1834">Erste Version</span><span class="sxs-lookup"><span data-stu-id="672ec-1834">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1835">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1835">Network</span></span>

* <span data-ttu-id="672ec-1836">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-1836">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="672ec-1837">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-1837">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="672ec-1838">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-1838">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="672ec-1839">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="672ec-1839">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1840">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1840">Profile</span></span>

* <span data-ttu-id="672ec-1841">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="672ec-1841">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-1842">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-1842">Storage</span></span>

* <span data-ttu-id="672ec-1843">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-1843">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-1844">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-1844">VM</span></span>

* <span data-ttu-id="672ec-1845">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1845">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="672ec-1846">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1846">Exposed `list-skus` command</span></span>
* <span data-ttu-id="672ec-1847">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="672ec-1847">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="672ec-1848">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="672ec-1848">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="672ec-1849">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1849">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="672ec-1850">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-1850">July 28, 2017</span></span>

<span data-ttu-id="672ec-1851">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="672ec-1851">Version 2.0.12</span></span>

* <span data-ttu-id="672ec-1852">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1852">Added container commands</span></span>
* <span data-ttu-id="672ec-1853">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1853">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="672ec-1854">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-1854">Core</span></span>

* <span data-ttu-id="672ec-1855">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="672ec-1855">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="672ec-1856">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1856">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="672ec-1857">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="672ec-1857">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="672ec-1858">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="672ec-1858">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="672ec-1859">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="672ec-1859">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="672ec-1860">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="672ec-1860">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="672ec-1861">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="672ec-1861">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="672ec-1862">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="672ec-1862">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="672ec-1863">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="672ec-1863">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="672ec-1864">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1864">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="672ec-1865">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="672ec-1865">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="672ec-1866">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="672ec-1866">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="672ec-1867">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="672ec-1867">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="672ec-1868">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="672ec-1868">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="672ec-1869">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="672ec-1869">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="672ec-1870">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="672ec-1870">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="672ec-1871">ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1871">ACR</span></span>

* <span data-ttu-id="672ec-1872">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1872">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="672ec-1873">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="672ec-1873">Support SKU update for managed registries</span></span>
* <span data-ttu-id="672ec-1874">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1874">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="672ec-1875">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1875">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="672ec-1876">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1876">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="672ec-1877">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1877">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-1878">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-1878">ACS</span></span>

* <span data-ttu-id="672ec-1879">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="672ec-1879">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-1880">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-1880">Appservice</span></span>

* <span data-ttu-id="672ec-1881">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="672ec-1881">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="672ec-1882">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="672ec-1882">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="672ec-1883">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="672ec-1883">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="672ec-1884">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="672ec-1884">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="672ec-1885">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="672ec-1885">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="672ec-1886">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="672ec-1886">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="672ec-1887">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="672ec-1887">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="672ec-1888">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="672ec-1888">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="672ec-1889">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1889">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="672ec-1890">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="672ec-1890">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="672ec-1891">Batch</span><span class="sxs-lookup"><span data-stu-id="672ec-1891">Batch</span></span>

* <span data-ttu-id="672ec-1892">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1892">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="672ec-1893">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1893">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="672ec-1894">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1894">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="672ec-1895">CDN</span><span class="sxs-lookup"><span data-stu-id="672ec-1895">CDN</span></span>

* <span data-ttu-id="672ec-1896">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="672ec-1896">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="672ec-1897">Cloud</span><span class="sxs-lookup"><span data-stu-id="672ec-1897">Cloud</span></span>

* <span data-ttu-id="672ec-1898">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="672ec-1898">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="672ec-1899">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="672ec-1899">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="672ec-1900">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="672ec-1900">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="672ec-1901">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="672ec-1901">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="672ec-1902">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="672ec-1902">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-1903">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-1903">CosmosDB</span></span>

* <span data-ttu-id="672ec-1904">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="672ec-1904">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="672ec-1905">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1905">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="672ec-1906">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="672ec-1906">Data Lake Analytics</span></span>

* <span data-ttu-id="672ec-1907">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1907">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="672ec-1908">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1908">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="672ec-1909">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1909">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="672ec-1910">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="672ec-1910">Data Lake Store</span></span>

* <span data-ttu-id="672ec-1911">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1911">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="672ec-1912">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="672ec-1912">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="672ec-1913">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1913">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="672ec-1914">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="672ec-1914">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="672ec-1915">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="672ec-1915">Interactive</span></span>

* <span data-ttu-id="672ec-1916">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1916">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="672ec-1917">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1917">Increased test coverage</span></span>
* <span data-ttu-id="672ec-1918">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-1918">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="672ec-1919">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="672ec-1919">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="672ec-1920">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="672ec-1920">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="672ec-1921">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="672ec-1921">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="672ec-1922">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="672ec-1922">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="672ec-1923">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1923">Added `--progress` flag</span></span>
* <span data-ttu-id="672ec-1924">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1924">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="672ec-1925">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="672ec-1925">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="672ec-1926">IoT</span><span class="sxs-lookup"><span data-stu-id="672ec-1926">IoT</span></span>

* <span data-ttu-id="672ec-1927">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="672ec-1927">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="672ec-1928">(3934)</span><span class="sxs-lookup"><span data-stu-id="672ec-1928">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="672ec-1929">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="672ec-1929">Key vault</span></span>

* <span data-ttu-id="672ec-1930">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="672ec-1930">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="672ec-1931">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="672ec-1931">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="672ec-1932">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="672ec-1932">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="672ec-1933">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="672ec-1933">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="672ec-1934">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="672ec-1934">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="672ec-1935">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="672ec-1935">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="672ec-1936">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1936">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="672ec-1937">(3307)</span><span class="sxs-lookup"><span data-stu-id="672ec-1937">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="672ec-1938">Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-1938">Lab</span></span>

* <span data-ttu-id="672ec-1939">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1939">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="672ec-1940">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1940">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-1941">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-1941">Monitor</span></span>

* <span data-ttu-id="672ec-1942">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="672ec-1942">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="672ec-1943">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1943">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="672ec-1944">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1944">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="672ec-1945">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1945">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="672ec-1946">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="672ec-1946">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="672ec-1947">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="672ec-1947">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="672ec-1948">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="672ec-1948">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="672ec-1949">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="672ec-1949">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="672ec-1950">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="672ec-1950">`location` no longer required</span></span>
  * <span data-ttu-id="672ec-1951">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="672ec-1951">Add name and ID support for target</span></span>
  * <span data-ttu-id="672ec-1952">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="672ec-1952">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="672ec-1953">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="672ec-1953">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="672ec-1954">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="672ec-1954">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="672ec-1955">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="672ec-1955">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="672ec-1956">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="672ec-1956">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="672ec-1957">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1957">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="672ec-1958">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-1958">Network</span></span>

* <span data-ttu-id="672ec-1959">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1959">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="672ec-1960">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1960">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="672ec-1961">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="672ec-1961">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="672ec-1962">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="672ec-1962">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="672ec-1963">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="672ec-1963">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="672ec-1964">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1964">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="672ec-1965">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="672ec-1965">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="672ec-1966">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="672ec-1966">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="672ec-1967">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="672ec-1967">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="672ec-1968">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="672ec-1968">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="672ec-1969">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1969">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="672ec-1970">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1970">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="672ec-1971">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="672ec-1971">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="672ec-1972">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1972">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="672ec-1973">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1973">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="672ec-1974">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-1974">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="672ec-1975">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="672ec-1975">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="672ec-1976">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-1976">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="672ec-1977">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1977">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="672ec-1978">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1978">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="672ec-1979">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="672ec-1979">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="672ec-1980">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="672ec-1980">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="672ec-1981">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1981">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="672ec-1982">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="672ec-1982">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="672ec-1983">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="672ec-1983">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="672ec-1984">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="672ec-1984">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="672ec-1985">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="672ec-1985">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-1986">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-1986">Profile</span></span>

* <span data-ttu-id="672ec-1987">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="672ec-1987">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="672ec-1988">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="672ec-1988">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="672ec-1989">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="672ec-1989">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="672ec-1990">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-1990">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="672ec-1991">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="672ec-1991">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="672ec-1992">RDBMS</span><span class="sxs-lookup"><span data-stu-id="672ec-1992">RDBMS</span></span>

* <span data-ttu-id="672ec-1993">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="672ec-1993">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="672ec-1994">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="672ec-1994">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="672ec-1995">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="672ec-1995">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="672ec-1996">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="672ec-1996">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-1997">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-1997">Resource</span></span>

* <span data-ttu-id="672ec-1998">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1998">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="672ec-1999">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="672ec-1999">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="672ec-2000">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-2000">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="672ec-2001">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="672ec-2001">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="672ec-2002">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="672ec-2002">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="672ec-2003">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="672ec-2003">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="672ec-2004">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="672ec-2004">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="672ec-2005">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-2005">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="672ec-2006">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-2006">Role</span></span>

* <span data-ttu-id="672ec-2007">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="672ec-2007">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="672ec-2008">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="672ec-2008">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="672ec-2009">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="672ec-2009">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="672ec-2010">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="672ec-2010">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="672ec-2011">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-2011">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="672ec-2012">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="672ec-2012">Service Fabric</span></span>
* <span data-ttu-id="672ec-2013">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="672ec-2013">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="672ec-2014">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="672ec-2014">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="672ec-2015">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="672ec-2015">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-2016">SQL</span></span>

* <span data-ttu-id="672ec-2017">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-2017">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="672ec-2018">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="672ec-2018">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="672ec-2019">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-2019">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-2020">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-2020">Storage</span></span>

* <span data-ttu-id="672ec-2021">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="672ec-2021">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="672ec-2022">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="672ec-2022">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="672ec-2023">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="672ec-2023">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="672ec-2024">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="672ec-2024">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="672ec-2025">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="672ec-2025">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="672ec-2026">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="672ec-2026">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-2027">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-2027">VM</span></span>

* <span data-ttu-id="672ec-2028">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="672ec-2028">Support configuring nsg</span></span>
* <span data-ttu-id="672ec-2029">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-2029">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="672ec-2030">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="672ec-2030">Support managed service identities</span></span>
* <span data-ttu-id="672ec-2031">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="672ec-2031">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="672ec-2032">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="672ec-2032">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="672ec-2033">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-2033">May 10, 2017</span></span>

<span data-ttu-id="672ec-2034">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="672ec-2034">Version 2.0.6</span></span>

* <span data-ttu-id="672ec-2035">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="672ec-2035">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="672ec-2036">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="672ec-2036">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="672ec-2037">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="672ec-2037">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="672ec-2038">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-2038">Include Cognitive Services module</span></span>
* <span data-ttu-id="672ec-2039">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-2039">Include Service Fabric module</span></span>
* <span data-ttu-id="672ec-2040">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="672ec-2040">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="672ec-2041">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="672ec-2041">Add support for CDN commands</span></span>
* <span data-ttu-id="672ec-2042">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="672ec-2042">Remove Container module</span></span>
* <span data-ttu-id="672ec-2043">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="672ec-2043">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="672ec-2044">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="672ec-2044">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="672ec-2045">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-2045">Core</span></span>

* <span data-ttu-id="672ec-2046">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="672ec-2046">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="672ec-2047">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="672ec-2047">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="672ec-2048">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="672ec-2048">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="672ec-2049">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="672ec-2049">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="672ec-2050">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="672ec-2050">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="672ec-2051">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="672ec-2051">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="672ec-2052">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="672ec-2052">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="672ec-2053">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="672ec-2053">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="672ec-2054">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="672ec-2054">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="672ec-2055">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="672ec-2055">core: Improved performance</span></span>
* <span data-ttu-id="672ec-2056">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="672ec-2056">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="672ec-2057">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="672ec-2057">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-2058">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-2058">ACS</span></span>

* <span data-ttu-id="672ec-2059">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="672ec-2059">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="672ec-2060">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="672ec-2060">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="672ec-2061">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="672ec-2061">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="672ec-2062">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="672ec-2062">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-2063">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-2063">AppService</span></span>

* <span data-ttu-id="672ec-2064">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="672ec-2064">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="672ec-2065">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="672ec-2065">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="672ec-2066">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="672ec-2066">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="672ec-2067">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="672ec-2067">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="672ec-2068">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="672ec-2068">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="672ec-2069">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="672ec-2069">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="672ec-2070">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="672ec-2070">support slot swap with preview</span></span>
* <span data-ttu-id="672ec-2071">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="672ec-2071">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="672ec-2072">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="672ec-2072">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="672ec-2073">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="672ec-2073">CosmosDB</span></span>

* <span data-ttu-id="672ec-2074">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="672ec-2074">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="672ec-2075">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="672ec-2075">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="672ec-2076">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="672ec-2076">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="672ec-2077">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="672ec-2077">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="672ec-2078">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="672ec-2078">Data Lake Analytics</span></span>

* <span data-ttu-id="672ec-2079">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="672ec-2079">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="672ec-2080">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="672ec-2080">Add support for new catalog item type: package.</span></span> <span data-ttu-id="672ec-2081">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="672ec-2081">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="672ec-2082">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="672ec-2082">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="672ec-2083">Table</span><span class="sxs-lookup"><span data-stu-id="672ec-2083">Table</span></span>
  * <span data-ttu-id="672ec-2084">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="672ec-2084">Table valued function</span></span>
  * <span data-ttu-id="672ec-2085">Sicht</span><span class="sxs-lookup"><span data-stu-id="672ec-2085">View</span></span>
  * <span data-ttu-id="672ec-2086">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="672ec-2086">Table Statistics.</span></span> <span data-ttu-id="672ec-2087">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="672ec-2087">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="672ec-2088">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="672ec-2088">Data Lake Store</span></span>

* <span data-ttu-id="672ec-2089">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-2089">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="672ec-2090">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="672ec-2090">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="672ec-2091">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="672ec-2091">missed help for access show.</span></span> <span data-ttu-id="672ec-2092">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="672ec-2092">adding it.</span></span> <span data-ttu-id="672ec-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="672ec-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="672ec-2094">Suchen</span><span class="sxs-lookup"><span data-stu-id="672ec-2094">Find</span></span>

* <span data-ttu-id="672ec-2095">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="672ec-2095">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="672ec-2096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="672ec-2096">KeyVault</span></span>

* <span data-ttu-id="672ec-2097">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="672ec-2097">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="672ec-2098">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="672ec-2098">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="672ec-2099">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="672ec-2099">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="672ec-2100">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="672ec-2100">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="672ec-2101">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="672ec-2101">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="672ec-2102">Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-2102">Lab</span></span>

* <span data-ttu-id="672ec-2103">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="672ec-2103">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="672ec-2104">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-2104">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="672ec-2105">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="672ec-2105">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="672ec-2106">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="672ec-2106">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="672ec-2107">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="672ec-2107">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="672ec-2108">Überwachen</span><span class="sxs-lookup"><span data-stu-id="672ec-2108">Monitor</span></span>

* <span data-ttu-id="672ec-2109">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="672ec-2109">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="672ec-2110">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="672ec-2110">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="672ec-2111">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-2111">Network</span></span>

* <span data-ttu-id="672ec-2112">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="672ec-2112">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="672ec-2113">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="672ec-2113">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="672ec-2114">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="672ec-2114">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="672ec-2115">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="672ec-2115">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="672ec-2116">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="672ec-2116">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="672ec-2117">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="672ec-2117">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="672ec-2118">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="672ec-2118">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="672ec-2119">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="672ec-2119">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="672ec-2120">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="672ec-2120">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="672ec-2121">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="672ec-2121">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="672ec-2122">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="672ec-2122">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="672ec-2123">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="672ec-2123">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="672ec-2124">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="672ec-2124">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="672ec-2125">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="672ec-2125">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="672ec-2126">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="672ec-2126">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="672ec-2127">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="672ec-2127">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="672ec-2128">Profil</span><span class="sxs-lookup"><span data-stu-id="672ec-2128">Profile</span></span>

* <span data-ttu-id="672ec-2129">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="672ec-2129">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="672ec-2130">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="672ec-2130">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="672ec-2131">Redis</span><span class="sxs-lookup"><span data-stu-id="672ec-2131">Redis</span></span>

* <span data-ttu-id="672ec-2132">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="672ec-2132">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="672ec-2133">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="672ec-2133">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="672ec-2134">Ressource</span><span class="sxs-lookup"><span data-stu-id="672ec-2134">Resource</span></span>

* <span data-ttu-id="672ec-2135">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="672ec-2135">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="672ec-2136">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="672ec-2136">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="672ec-2137">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="672ec-2137">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="672ec-2138">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="672ec-2138">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="672ec-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="672ec-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="672ec-2140">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="672ec-2140">Add docs for az lock update.</span></span> <span data-ttu-id="672ec-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="672ec-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="672ec-2142">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="672ec-2142">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="672ec-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="672ec-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="672ec-2144">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="672ec-2144">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="672ec-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="672ec-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="672ec-2146">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="672ec-2146">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="672ec-2147">Rolle</span><span class="sxs-lookup"><span data-stu-id="672ec-2147">Role</span></span>

* <span data-ttu-id="672ec-2148">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="672ec-2148">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="672ec-2149">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="672ec-2149">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="672ec-2150">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="672ec-2150">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="672ec-2151">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="672ec-2151">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="672ec-2152">SQL</span><span class="sxs-lookup"><span data-stu-id="672ec-2152">SQL</span></span>

* <span data-ttu-id="672ec-2153">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="672ec-2153">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="672ec-2154">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="672ec-2154">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="672ec-2155">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-2155">Storage</span></span>

* <span data-ttu-id="672ec-2156">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="672ec-2156">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="672ec-2157">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="672ec-2157">Add support for incremental blob copy</span></span>
* <span data-ttu-id="672ec-2158">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="672ec-2158">Add support for large block blob upload</span></span>
* <span data-ttu-id="672ec-2159">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="672ec-2159">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-2160">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-2160">VM</span></span>

* <span data-ttu-id="672ec-2161">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="672ec-2161">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="672ec-2162">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="672ec-2162">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="672ec-2163">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="672ec-2163">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="672ec-2164">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="672ec-2164">az vm/vmss disk</span></span>
  3. <span data-ttu-id="672ec-2165">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="672ec-2165">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="672ec-2166">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="672ec-2166">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="672ec-2167">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="672ec-2167">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="672ec-2168">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-2168">April 3, 2017</span></span>

<span data-ttu-id="672ec-2169">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="672ec-2169">Version 2.0.2</span></span>

<span data-ttu-id="672ec-2170">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="672ec-2170">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="672ec-2171">Core</span><span class="sxs-lookup"><span data-stu-id="672ec-2171">Core</span></span>

* <span data-ttu-id="672ec-2172">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="672ec-2172">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="672ec-2173">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="672ec-2173">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="672ec-2174">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="672ec-2174">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="672ec-2175">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="672ec-2175">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="672ec-2176">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="672ec-2176">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="672ec-2177">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="672ec-2177">Add prompting for missing template parameters.</span></span> <span data-ttu-id="672ec-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="672ec-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="672ec-2179">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="672ec-2179">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="672ec-2180">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="672ec-2180">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="672ec-2181">ACS</span><span class="sxs-lookup"><span data-stu-id="672ec-2181">ACS</span></span>

* <span data-ttu-id="672ec-2182">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="672ec-2182">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="672ec-2183">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="672ec-2183">Add support for ssh key password prompting.</span></span> <span data-ttu-id="672ec-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="672ec-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="672ec-2185">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="672ec-2185">Add support for windows clusters.</span></span> <span data-ttu-id="672ec-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="672ec-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="672ec-2187">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="672ec-2187">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="672ec-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="672ec-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="672ec-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="672ec-2189">AppService</span></span>

* <span data-ttu-id="672ec-2190">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="672ec-2190">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="672ec-2191">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="672ec-2191">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="672ec-2192">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="672ec-2192">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="672ec-2193">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="672ec-2193">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="672ec-2194">DataLake</span><span class="sxs-lookup"><span data-stu-id="672ec-2194">DataLake</span></span>

* <span data-ttu-id="672ec-2195">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-2195">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="672ec-2196">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="672ec-2196">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="672ec-2197">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="672ec-2197">DocuemntDB</span></span>

* <span data-ttu-id="672ec-2198">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="672ec-2198">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="672ec-2199">VM</span><span class="sxs-lookup"><span data-stu-id="672ec-2199">VM</span></span>

* <span data-ttu-id="672ec-2200">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="672ec-2200">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="672ec-2201">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="672ec-2201">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="672ec-2202">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="672ec-2202">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="672ec-2203">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="672ec-2203">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="672ec-2204">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="672ec-2204">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="672ec-2205">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="672ec-2205">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="672ec-2206">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="672ec-2206">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="672ec-2207">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="672ec-2207">February 27, 2017</span></span>

<span data-ttu-id="672ec-2208">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="672ec-2208">Version 2.0.0</span></span>

<span data-ttu-id="672ec-2209">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="672ec-2209">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="672ec-2210">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="672ec-2210">Container Service (acs)</span></span>
- <span data-ttu-id="672ec-2211">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="672ec-2211">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="672ec-2212">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="672ec-2212">Networking</span></span>
- <span data-ttu-id="672ec-2213">Storage</span><span class="sxs-lookup"><span data-stu-id="672ec-2213">Storage</span></span>

<span data-ttu-id="672ec-2214">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="672ec-2214">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="672ec-2215">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="672ec-2215">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="672ec-2216">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="672ec-2216">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="672ec-2217">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="672ec-2217">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="672ec-2218">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="672ec-2218">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="672ec-2219">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="672ec-2219">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="672ec-2220">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="672ec-2220">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="672ec-2221">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="672ec-2221">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="672ec-2222">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="672ec-2222">Provide feedback from the command line with the `az feedback` command</span></span>


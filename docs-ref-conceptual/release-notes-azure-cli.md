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
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158354"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="6f318-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6f318-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="6f318-104">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="6f318-104">February 12, 2019</span></span>

<span data-ttu-id="6f318-105">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="6f318-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="6f318-106">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-106">Core</span></span>

* <span data-ttu-id="6f318-107">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="6f318-108">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-109">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-109">ACR</span></span>
* <span data-ttu-id="6f318-110">[WICHTIGE ÄNDERUNG] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="6f318-111">[WICHTIGE ÄNDERUNG] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-112">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-112">ACS</span></span>
* <span data-ttu-id="6f318-113">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="6f318-114">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="6f318-115">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="6f318-116">AMS</span><span class="sxs-lookup"><span data-stu-id="6f318-116">AMS</span></span>
* <span data-ttu-id="6f318-117">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="6f318-118">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-119">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-119">Appservice</span></span>
* <span data-ttu-id="6f318-120">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="6f318-121">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="6f318-122">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6f318-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="6f318-123">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="6f318-124">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="6f318-125">Botservice</span><span class="sxs-lookup"><span data-stu-id="6f318-125">Botservice</span></span>
* <span data-ttu-id="6f318-126">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6f318-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="6f318-127">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="6f318-128">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="6f318-129">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="6f318-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="6f318-130">[VERALTET] Das `--proj-name`-Argument wurde zugunsten von `--proj-file-path` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="6f318-131">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="6f318-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="6f318-132">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="6f318-133">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="6f318-134">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="6f318-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="6f318-135">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f318-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="6f318-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6f318-136">Key Vault</span></span>
* <span data-ttu-id="6f318-137">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="6f318-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-138">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-138">Monitor</span></span>
* <span data-ttu-id="6f318-139">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-140">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-140">Network</span></span>
* <span data-ttu-id="6f318-141">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="6f318-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="6f318-142">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6f318-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="6f318-143">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6f318-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="6f318-144">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6f318-145">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="6f318-145">Policy Insights</span></span>
* <span data-ttu-id="6f318-146">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6f318-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-147">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-147">RDBMS</span></span>
* <span data-ttu-id="6f318-148">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="6f318-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="6f318-149">Redis</span><span class="sxs-lookup"><span data-stu-id="6f318-149">Redis</span></span>
* <span data-ttu-id="6f318-150">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="6f318-151">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="6f318-152">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="6f318-153">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="6f318-154">[WICHTIGE ÄNDERUNG] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="6f318-155">[WICHTIGE ÄNDERUNG] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="6f318-156">[VERALTET] Warnmeldung für die Deaktivierung von des Befehls `redis import-method` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="6f318-157">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-157">Role</span></span>
* <span data-ttu-id="6f318-158">[WICHTIGE ÄNDERUNG] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="6f318-159">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="6f318-159">SQL VM</span></span>
* <span data-ttu-id="6f318-160">[VERALTET] Das `--boostrap-acc-pwd`-Argument wurde aufgrund eines Tippfehlers als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-161">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-161">VM</span></span>
* <span data-ttu-id="6f318-162">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="6f318-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="6f318-163">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="6f318-164">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="6f318-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="6f318-165">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="6f318-166">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6f318-166">January 31, 2019</span></span>

<span data-ttu-id="6f318-167">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="6f318-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="6f318-168">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-168">Core</span></span>

* <span data-ttu-id="6f318-169">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="6f318-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="6f318-170">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6f318-170">January 28, 2019</span></span>

<span data-ttu-id="6f318-171">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="6f318-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-172">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-172">ACR</span></span>
* <span data-ttu-id="6f318-173">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-174">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-174">ACS</span></span>
* <span data-ttu-id="6f318-175">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6f318-176">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="6f318-177">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="6f318-178">AMS</span><span class="sxs-lookup"><span data-stu-id="6f318-178">AMS</span></span>
* <span data-ttu-id="6f318-179">[WICHTIGE ÄNDERUNG] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="6f318-180">[WICHTIGE ÄNDERUNG] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-181">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-181">Appservice</span></span>
* <span data-ttu-id="6f318-182">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="6f318-183">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="6f318-184">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="6f318-185">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-185">Container</span></span>
* <span data-ttu-id="6f318-186">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-186">Added `container start` command</span></span>
* <span data-ttu-id="6f318-187">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="6f318-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6f318-188">EventGrid</span><span class="sxs-lookup"><span data-stu-id="6f318-188">EventGrid</span></span>
* <span data-ttu-id="6f318-189">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="6f318-190">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="6f318-191">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="6f318-192">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="6f318-193">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6f318-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6f318-194">HDInsight</span></span>
* <span data-ttu-id="6f318-195">[WICHTIGE ÄNDERUNG] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="6f318-196">[WICHTIGE ÄNDERUNG] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="6f318-197">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="6f318-198">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="6f318-199">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="6f318-200">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-201">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-201">IoT</span></span>
* <span data-ttu-id="6f318-202">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="6f318-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="6f318-203">Kusto</span></span>
* <span data-ttu-id="6f318-204">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6f318-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-205">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-205">Monitor</span></span>
* <span data-ttu-id="6f318-206">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-207">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-207">Profile</span></span>
* <span data-ttu-id="6f318-208">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6f318-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-209">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-209">Network</span></span>
* <span data-ttu-id="6f318-210">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="6f318-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="6f318-211">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="6f318-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-212">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-212">Resource</span></span>
* <span data-ttu-id="6f318-213">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="6f318-214">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="6f318-215">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="6f318-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="6f318-216">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6f318-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-217">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-217">Storage</span></span>
* <span data-ttu-id="6f318-218">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="6f318-219">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-220">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-220">VM</span></span>
* <span data-ttu-id="6f318-221">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="6f318-222">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="6f318-223">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6f318-223">January 15, 2019</span></span>

<span data-ttu-id="6f318-224">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="6f318-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-225">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-225">ACR</span></span>
* <span data-ttu-id="6f318-226">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="6f318-227">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="6f318-228">[VERALTET] Parameter `--resource-group` wurde in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="6f318-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="6f318-229">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-229">ACS</span></span>
* <span data-ttu-id="6f318-230">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-231">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-231">Appservice</span></span>
* <span data-ttu-id="6f318-232">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="6f318-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="6f318-233">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="6f318-234">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="6f318-235">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="6f318-236">Botservice</span><span class="sxs-lookup"><span data-stu-id="6f318-236">Botservice</span></span>
* <span data-ttu-id="6f318-237">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="6f318-238">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6f318-238">Configure</span></span>
* <span data-ttu-id="6f318-239">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-240">CosmosDB</span></span>
* <span data-ttu-id="6f318-241">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6f318-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6f318-242">HDInsight</span></span>
* <span data-ttu-id="6f318-243">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-243">Added commands for managing applications</span></span>
* <span data-ttu-id="6f318-244">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="6f318-245">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="6f318-246">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="6f318-247">[WICHTIGE ÄNDERUNG] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-248">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-248">Network</span></span>
* <span data-ttu-id="6f318-249">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="6f318-250">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="6f318-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="6f318-251">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="6f318-252">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="6f318-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="6f318-253">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-253">Role</span></span>
* <span data-ttu-id="6f318-254">[VERALTET] Das `--password`-Argument wurde für `create-for-rbac` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="6f318-255">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="6f318-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="6f318-256">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="6f318-256">Security</span></span>
* <span data-ttu-id="6f318-257">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-258">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-258">Storage</span></span>
* <span data-ttu-id="6f318-259">[WICHTIGE ÄNDERUNG] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="6f318-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="6f318-260">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="6f318-261">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="6f318-262">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="6f318-263">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-264">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-264">VM</span></span>
* <span data-ttu-id="6f318-265">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f318-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="6f318-266">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6f318-267">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="6f318-268">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="6f318-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="6f318-269">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="6f318-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="6f318-270">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="6f318-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="6f318-271">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-271">December 20, 2018</span></span>

<span data-ttu-id="6f318-272">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="6f318-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="6f318-273">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-273">Appservice</span></span>
* <span data-ttu-id="6f318-274">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="6f318-275">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="6f318-276">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6f318-277">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="6f318-277">IoTCentral</span></span>
* <span data-ttu-id="6f318-278">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="6f318-279">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-279">Role</span></span>
* <span data-ttu-id="6f318-280">[WICHTIGE ÄNDERUNG] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="6f318-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-281">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-281">SQL</span></span>
* <span data-ttu-id="6f318-282">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-283">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-283">VM</span></span>
* <span data-ttu-id="6f318-284">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="6f318-285">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-285">December 18, 2018</span></span>

<span data-ttu-id="6f318-286">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="6f318-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="6f318-287">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-287">ACR</span></span>
* <span data-ttu-id="6f318-288">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="6f318-289">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="6f318-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="6f318-290">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-291">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-291">ACS</span></span>
* <span data-ttu-id="6f318-292">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6f318-293">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="6f318-294">[VERALTET] `az acs`-Befehle als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="6f318-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="6f318-295">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="6f318-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="6f318-296">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="6f318-297">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-298">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-298">Appservice</span></span>
* <span data-ttu-id="6f318-299">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="6f318-300">Botservice</span><span class="sxs-lookup"><span data-stu-id="6f318-300">Botservice</span></span>
* <span data-ttu-id="6f318-301">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="6f318-302">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="6f318-303">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="6f318-304">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="6f318-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="6f318-305">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="6f318-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-306">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-306">Consumption</span></span>
* <span data-ttu-id="6f318-307">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-308">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-308">CosmosDB</span></span>
* <span data-ttu-id="6f318-309">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="6f318-310">Karten</span><span class="sxs-lookup"><span data-stu-id="6f318-310">Maps</span></span>
* <span data-ttu-id="6f318-311">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-312">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-312">Network</span></span>
* <span data-ttu-id="6f318-313">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="6f318-314">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6f318-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-315">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-315">Resource</span></span>
* <span data-ttu-id="6f318-316">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="6f318-317">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-318">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-318">Storage</span></span>
*  <span data-ttu-id="6f318-319">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-320">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-320">VM</span></span>
* <span data-ttu-id="6f318-321">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="6f318-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="6f318-322">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-322">December 4, 2018</span></span>

<span data-ttu-id="6f318-323">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="6f318-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="6f318-324">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-324">Core</span></span>
* <span data-ttu-id="6f318-325">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="6f318-326">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-327">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-327">Appservice</span></span>
* <span data-ttu-id="6f318-328">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f318-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="6f318-329">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="6f318-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="6f318-330">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-330">Network</span></span>
* <span data-ttu-id="6f318-331">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="6f318-332">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-332">Role</span></span>
* <span data-ttu-id="6f318-333">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="6f318-334">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-334">VM</span></span>
* <span data-ttu-id="6f318-335">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="6f318-336">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="6f318-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="6f318-337">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6f318-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="6f318-338">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="6f318-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="6f318-339">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-339">November 20, 2018</span></span>

<span data-ttu-id="6f318-340">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="6f318-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="6f318-341">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-341">Core</span></span>
* <span data-ttu-id="6f318-342">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-343">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-343">ACR</span></span>
* <span data-ttu-id="6f318-344">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-344">Added context token to task step</span></span>
* <span data-ttu-id="6f318-345">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="6f318-346">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-347">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-347">Appservice</span></span>
* <span data-ttu-id="6f318-348">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="6f318-349">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="6f318-349">Updated the default `node_version`.</span></span> <span data-ttu-id="6f318-350">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="6f318-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="6f318-351">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="6f318-352">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="6f318-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6f318-353">IotCentral</span><span class="sxs-lookup"><span data-stu-id="6f318-353">IotCentral</span></span>
* <span data-ttu-id="6f318-354">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-355">KeyVault</span></span>
* <span data-ttu-id="6f318-356">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="6f318-357">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-357">Network</span></span>
* <span data-ttu-id="6f318-358">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="6f318-359">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="6f318-360">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="6f318-361">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6f318-362">Rdbms</span></span>
* <span data-ttu-id="6f318-363">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="6f318-364">RBAC</span><span class="sxs-lookup"><span data-stu-id="6f318-364">Rbac</span></span>
* <span data-ttu-id="6f318-365">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="6f318-366">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="6f318-367">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-367">Storage</span></span>
* <span data-ttu-id="6f318-368">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="6f318-369">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="6f318-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="6f318-370">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="6f318-371">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-372">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-372">VM</span></span>
* <span data-ttu-id="6f318-373">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="6f318-374">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="6f318-375">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6f318-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="6f318-376">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="6f318-377">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="6f318-378">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="6f318-379">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="6f318-380">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-380">November 6, 2018</span></span>

<span data-ttu-id="6f318-381">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="6f318-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="6f318-382">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-382">Core</span></span>
* <span data-ttu-id="6f318-383">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-384">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-384">ACR</span></span>
* <span data-ttu-id="6f318-385">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="6f318-386">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-387">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-387">ACS</span></span>
* <span data-ttu-id="6f318-388">[WICHTIGE ÄNDERUNG] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="6f318-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="6f318-389">Advisor</span><span class="sxs-lookup"><span data-stu-id="6f318-389">Advisor</span></span>
* <span data-ttu-id="6f318-390">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="6f318-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="6f318-391">AMS</span><span class="sxs-lookup"><span data-stu-id="6f318-391">AMS</span></span>
* <span data-ttu-id="6f318-392">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="6f318-393">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="6f318-394">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="6f318-395">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="6f318-396">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="6f318-397">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="6f318-398">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="6f318-399">[WICHTIGE ÄNDERUNG] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6f318-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="6f318-400">[WICHTIGE ÄNDERUNG] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="6f318-401">[WICHTIGE ÄNDERUNG] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="6f318-402">[WICHTIGE ÄNDERUNG] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6f318-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="6f318-403">[WICHTIGE ÄNDERUNG] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6f318-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="6f318-404">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="6f318-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="6f318-405">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="6f318-406">[WICHTIGE ÄNDERUNG] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6f318-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="6f318-407">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="6f318-408">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="6f318-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-409">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-409">AppService</span></span>
* <span data-ttu-id="6f318-410">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="6f318-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="6f318-411">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6f318-411">Configure</span></span>
* <span data-ttu-id="6f318-412">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="6f318-413">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-413">Container</span></span>
* <span data-ttu-id="6f318-414">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="6f318-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="6f318-415">EventHub</span><span class="sxs-lookup"><span data-stu-id="6f318-415">EventHub</span></span>
* <span data-ttu-id="6f318-416">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-417">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-417">Interactive</span></span>
* <span data-ttu-id="6f318-418">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-419">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-419">Monitor</span></span>
* <span data-ttu-id="6f318-420">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-421">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-421">Network</span></span>
* <span data-ttu-id="6f318-422">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="6f318-423">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="6f318-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="6f318-424">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="6f318-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="6f318-425">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-425">Profile</span></span>
* <span data-ttu-id="6f318-426">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-427">RDBMS</span></span>
* <span data-ttu-id="6f318-428">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-429">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-429">Resource</span></span>
* <span data-ttu-id="6f318-430">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="6f318-431">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-431">Role</span></span>
* <span data-ttu-id="6f318-432">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="6f318-433">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="6f318-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="6f318-434">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-435">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-435">Storage</span></span>
* <span data-ttu-id="6f318-436">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="6f318-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-437">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-437">VM</span></span>
* <span data-ttu-id="6f318-438">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="6f318-439">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="6f318-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="6f318-440">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="6f318-441">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="6f318-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="6f318-442">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="6f318-443">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="6f318-444">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-444">October 23, 2018</span></span>

<span data-ttu-id="6f318-445">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="6f318-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="6f318-446">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-446">Core</span></span>
* <span data-ttu-id="6f318-447">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="6f318-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="6f318-448">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="6f318-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-449">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-449">ACR</span></span>
* <span data-ttu-id="6f318-450">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="6f318-451">CDN</span><span class="sxs-lookup"><span data-stu-id="6f318-451">CDN</span></span>
* <span data-ttu-id="6f318-452">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="6f318-453">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6f318-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="6f318-454">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-454">Container</span></span>
* <span data-ttu-id="6f318-455">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="6f318-456">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="6f318-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="6f318-457">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="6f318-458">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="6f318-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="6f318-459">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6f318-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="6f318-460">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="6f318-461">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-462">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-462">CosmosDB</span></span>
* <span data-ttu-id="6f318-463">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-464">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-464">Interactive</span></span>
* <span data-ttu-id="6f318-465">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="6f318-466">IoT Central</span><span class="sxs-lookup"><span data-stu-id="6f318-466">IoT Central</span></span>
* <span data-ttu-id="6f318-467">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="6f318-468">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f318-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-469">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-469">Monitor</span></span>
* <span data-ttu-id="6f318-470">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="6f318-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="6f318-471">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="6f318-472">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6f318-473">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="6f318-474">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="6f318-475">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="6f318-476">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="6f318-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="6f318-477">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6f318-478">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="6f318-479">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-480">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-480">Network</span></span>
* <span data-ttu-id="6f318-481">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="6f318-482">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="6f318-483">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6f318-483">ServiceBus</span></span>
* <span data-ttu-id="6f318-484">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-485">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-485">SQL</span></span>
* <span data-ttu-id="6f318-486">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="6f318-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-487">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-487">Storage</span></span>
* <span data-ttu-id="6f318-488">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="6f318-489">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-490">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-490">VM</span></span>
* <span data-ttu-id="6f318-491">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="6f318-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="6f318-492">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="6f318-493">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="6f318-494">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-494">October 16, 2018</span></span>

<span data-ttu-id="6f318-495">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="6f318-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-496">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-496">VM</span></span>
* <span data-ttu-id="6f318-497">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="6f318-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="6f318-498">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-498">October 9, 2018</span></span>

<span data-ttu-id="6f318-499">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="6f318-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="6f318-500">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-500">Core</span></span>
* <span data-ttu-id="6f318-501">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="6f318-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-502">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-502">ACR</span></span>
* <span data-ttu-id="6f318-503">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-504">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-504">ACS</span></span>
* <span data-ttu-id="6f318-505">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="6f318-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="6f318-506">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="6f318-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="6f318-507">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="6f318-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="6f318-508">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="6f318-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="6f318-509">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-509">Container</span></span>
* <span data-ttu-id="6f318-510">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="6f318-511">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="6f318-512">Event Hub</span><span class="sxs-lookup"><span data-stu-id="6f318-512">Event Hub</span></span>
* <span data-ttu-id="6f318-513">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="6f318-514">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="6f318-515">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6f318-515">Extensions</span></span>
* <span data-ttu-id="6f318-516">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="6f318-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6f318-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6f318-517">HDInsight</span></span>
* <span data-ttu-id="6f318-518">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-519">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-519">IoT</span></span>
* <span data-ttu-id="6f318-520">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-521">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-521">KeyVault</span></span>
* <span data-ttu-id="6f318-522">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="6f318-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="6f318-523">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-523">Network</span></span>
* <span data-ttu-id="6f318-524">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="6f318-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="6f318-525">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="6f318-525">See #6052</span></span>
* <span data-ttu-id="6f318-526">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="6f318-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="6f318-527">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="6f318-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="6f318-528">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="6f318-529">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="6f318-530">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6f318-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="6f318-531">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="6f318-532">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-532">Role</span></span>
* <span data-ttu-id="6f318-533">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="6f318-534">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="6f318-535">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6f318-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="6f318-536">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="6f318-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="6f318-537">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6f318-537">Service Bus</span></span>
* <span data-ttu-id="6f318-538">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-539">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-539">VM</span></span>
* <span data-ttu-id="6f318-540">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="6f318-541">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="6f318-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="6f318-542">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="6f318-543">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="6f318-544">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="6f318-545">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="6f318-546">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-546">September 21, 2018</span></span>

<span data-ttu-id="6f318-547">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="6f318-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-548">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-548">ACR</span></span>
* <span data-ttu-id="6f318-549">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-549">Added ACR Task commands</span></span>
* <span data-ttu-id="6f318-550">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-550">Added quick run command</span></span>
* <span data-ttu-id="6f318-551">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="6f318-552">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="6f318-553">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="6f318-554">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-555">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-555">ACS</span></span>
* <span data-ttu-id="6f318-556">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="6f318-557">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-558">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-558">AppService</span></span>

* <span data-ttu-id="6f318-559">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="6f318-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="6f318-560">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="6f318-561">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="6f318-562">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-563">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-563">Batch</span></span>
* <span data-ttu-id="6f318-564">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="6f318-565">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="6f318-566">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="6f318-567">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6f318-568">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-568">Batch AI</span></span> 
* <span data-ttu-id="6f318-569">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6f318-570">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6f318-570">Cognitive Services</span></span>
* <span data-ttu-id="6f318-571">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="6f318-572">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="6f318-573">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="6f318-574">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="6f318-575">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="6f318-576">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="6f318-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="6f318-577">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-577">Container</span></span>
* <span data-ttu-id="6f318-578">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="6f318-579">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="6f318-580">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="6f318-581">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="6f318-582">Data Lake</span><span class="sxs-lookup"><span data-stu-id="6f318-582">Datalake</span></span>
* <span data-ttu-id="6f318-583">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="6f318-584">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="6f318-584">Interactive Shell</span></span>
* <span data-ttu-id="6f318-585">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="6f318-586">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-587">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-587">IoT</span></span>
* <span data-ttu-id="6f318-588">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="6f318-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6f318-589">Key Vault</span></span>
* <span data-ttu-id="6f318-590">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="6f318-591">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-591">Network</span></span>
* <span data-ttu-id="6f318-592">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="6f318-593">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="6f318-594">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="6f318-595">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="6f318-596">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="6f318-597">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="6f318-598">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="6f318-599">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="6f318-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="6f318-600">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="6f318-601">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="6f318-602">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="6f318-603">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="6f318-604">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="6f318-605">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="6f318-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="6f318-606">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="6f318-607">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="6f318-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="6f318-608">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="6f318-609">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-610">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-610">RDBMS</span></span>
* <span data-ttu-id="6f318-611">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="6f318-612">Reservierung</span><span class="sxs-lookup"><span data-stu-id="6f318-612">Reservation</span></span>
* <span data-ttu-id="6f318-613">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="6f318-614">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="6f318-615">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="6f318-615">Manage App</span></span>
* <span data-ttu-id="6f318-616">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="6f318-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="6f318-617">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="6f318-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="6f318-618">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-618">Role</span></span>
* <span data-ttu-id="6f318-619">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="6f318-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="6f318-620">SignalR</span></span>
* <span data-ttu-id="6f318-621">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-622">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-622">Storage</span></span>
* <span data-ttu-id="6f318-623">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="6f318-624">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-625">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-625">VM</span></span>
* <span data-ttu-id="6f318-626">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="6f318-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="6f318-627">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="6f318-628">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-628">August 28, 2018</span></span>

<span data-ttu-id="6f318-629">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="6f318-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="6f318-630">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-630">Core</span></span>

* <span data-ttu-id="6f318-631">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="6f318-632">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-633">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-633">ACR</span></span>

* <span data-ttu-id="6f318-634">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="6f318-635">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="6f318-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-636">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-636">ACS</span></span>

* <span data-ttu-id="6f318-637">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="6f318-638">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="6f318-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-639">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-639">AppService</span></span>

* <span data-ttu-id="6f318-640">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="6f318-641">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="6f318-642">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="6f318-643">Backup</span><span class="sxs-lookup"><span data-stu-id="6f318-643">Backup</span></span>

* <span data-ttu-id="6f318-644">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="6f318-645">Botdienst</span><span class="sxs-lookup"><span data-stu-id="6f318-645">Bot Service</span></span>

* <span data-ttu-id="6f318-646">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="6f318-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6f318-647">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6f318-647">Cognitive Services</span></span>

* <span data-ttu-id="6f318-648">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="6f318-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-649">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-649">IoT</span></span>

* <span data-ttu-id="6f318-650">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-651">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-651">Monitor</span></span>

* <span data-ttu-id="6f318-652">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="6f318-653">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6f318-654">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-654">Network</span></span>

* <span data-ttu-id="6f318-655">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-656">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-656">Resource</span></span>

* <span data-ttu-id="6f318-657">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-658">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-658">Storage</span></span>

* <span data-ttu-id="6f318-659">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-660">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-660">VM</span></span>

* <span data-ttu-id="6f318-661">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6f318-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="6f318-662">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="6f318-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="6f318-663">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-663">Auguest 14, 2018</span></span>

<span data-ttu-id="6f318-664">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="6f318-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="6f318-665">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-665">Core</span></span>

* <span data-ttu-id="6f318-666">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="6f318-667">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="6f318-668">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="6f318-668">Telemetry</span></span>

* <span data-ttu-id="6f318-669">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="6f318-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-670">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-670">ACR</span></span>

* <span data-ttu-id="6f318-671">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="6f318-672">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-673">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-673">ACS</span></span>

* <span data-ttu-id="6f318-674">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="6f318-675">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6f318-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="6f318-676">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="6f318-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="6f318-677">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="6f318-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="6f318-678">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6f318-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="6f318-679">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-679">AppService</span></span>

* <span data-ttu-id="6f318-680">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="6f318-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="6f318-681">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="6f318-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-682">BatchAI</span></span>

* <span data-ttu-id="6f318-683">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6f318-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="6f318-684">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-684">Container</span></span>

* <span data-ttu-id="6f318-685">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="6f318-686">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-686">IoT</span></span>

* <span data-ttu-id="6f318-687">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="6f318-688">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="6f318-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="6f318-689">Iot Central</span><span class="sxs-lookup"><span data-stu-id="6f318-689">Iot Central</span></span>

* <span data-ttu-id="6f318-690">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-691">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-691">KeyVault</span></span>


* <span data-ttu-id="6f318-692">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="6f318-693">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="6f318-694">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="6f318-695">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="6f318-696">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="6f318-697">Relay</span><span class="sxs-lookup"><span data-stu-id="6f318-697">Relay</span></span>

* <span data-ttu-id="6f318-698">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-699">Sql</span><span class="sxs-lookup"><span data-stu-id="6f318-699">Sql</span></span>

* <span data-ttu-id="6f318-700">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-701">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-701">Storage</span></span>

* <span data-ttu-id="6f318-702">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="6f318-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="6f318-703">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="6f318-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="6f318-704">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="6f318-705">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="6f318-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="6f318-706">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="6f318-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-707">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-707">VM</span></span>

* <span data-ttu-id="6f318-708">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="6f318-709">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-709">July 31, 2018</span></span>

<span data-ttu-id="6f318-710">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="6f318-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-711">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-711">ACR</span></span>

* <span data-ttu-id="6f318-712">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="6f318-713">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-714">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-714">ACS</span></span>

* <span data-ttu-id="6f318-715">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-716">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-716">Batch</span></span>

* <span data-ttu-id="6f318-717">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6f318-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="6f318-718">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-718">Container</span></span>

* <span data-ttu-id="6f318-719">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="6f318-720">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-720">Network</span></span>

* <span data-ttu-id="6f318-721">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="6f318-722">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-722">Resource</span></span>

* <span data-ttu-id="6f318-723">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="6f318-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="6f318-724">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="6f318-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="6f318-725">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-725">Role</span></span>

* <span data-ttu-id="6f318-726">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="6f318-727">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6f318-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="6f318-728">Suchen,</span><span class="sxs-lookup"><span data-stu-id="6f318-728">Search</span></span>

* <span data-ttu-id="6f318-729">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="6f318-730">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6f318-730">Service Bus</span></span>

* <span data-ttu-id="6f318-731">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="6f318-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="6f318-732">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="6f318-733">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="6f318-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="6f318-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="6f318-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-735">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-735">Storage</span></span>

* <span data-ttu-id="6f318-736">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="6f318-737">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-738">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-738">VM</span></span>

* <span data-ttu-id="6f318-739">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="6f318-740">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="6f318-741">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="6f318-742">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="6f318-743">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-743">July 18, 2018</span></span>

<span data-ttu-id="6f318-744">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="6f318-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="6f318-745">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-745">Core</span></span>

* <span data-ttu-id="6f318-746">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="6f318-747">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="6f318-748">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="6f318-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-749">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-749">ACR</span></span>

* <span data-ttu-id="6f318-750">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="6f318-751">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="6f318-752">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="6f318-753">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-754">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-754">ACS</span></span>

* <span data-ttu-id="6f318-755">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="6f318-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-756">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-756">AppService</span></span>

* <span data-ttu-id="6f318-757">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-758">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-758">Batch</span></span>

* <span data-ttu-id="6f318-759">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="6f318-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="6f318-760">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6f318-761">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-761">Batch AI</span></span>

* <span data-ttu-id="6f318-762">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="6f318-763">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-763">Container</span></span>

* <span data-ttu-id="6f318-764">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="6f318-765">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="6f318-766">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-766">Network</span></span>

* <span data-ttu-id="6f318-767">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="6f318-768">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-768">Added `network nic wait`</span></span>
* <span data-ttu-id="6f318-769">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="6f318-770">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="6f318-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="6f318-771">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-771">Resource</span></span>

* <span data-ttu-id="6f318-772">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="6f318-773">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="6f318-774">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="6f318-775">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-776">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-776">SQL</span></span>

* <span data-ttu-id="6f318-777">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="6f318-778">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="6f318-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="6f318-779">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-780">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-780">Storage</span></span>

* <span data-ttu-id="6f318-781">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-782">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-782">VM</span></span>

* <span data-ttu-id="6f318-783">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="6f318-784">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="6f318-785">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6f318-786">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-786">July 3, 2018</span></span>

<span data-ttu-id="6f318-787">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="6f318-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="6f318-788">AKS</span><span class="sxs-lookup"><span data-stu-id="6f318-788">AKS</span></span>

* <span data-ttu-id="6f318-789">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6f318-790">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-790">July 3, 2018</span></span>

<span data-ttu-id="6f318-791">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="6f318-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="6f318-792">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-792">Core</span></span>

* <span data-ttu-id="6f318-793">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-794">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-794">ACR</span></span>

* <span data-ttu-id="6f318-795">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-795">Added polling build status</span></span>
* <span data-ttu-id="6f318-796">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="6f318-797">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-798">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-798">ACS</span></span>

* <span data-ttu-id="6f318-799">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="6f318-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="6f318-800">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="6f318-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="6f318-801">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="6f318-802">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="6f318-803">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="6f318-804">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="6f318-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="6f318-805">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-806">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-806">AppService</span></span>

* <span data-ttu-id="6f318-807">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="6f318-808">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="6f318-809">Backup</span><span class="sxs-lookup"><span data-stu-id="6f318-809">Backup</span></span>

* <span data-ttu-id="6f318-810">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="6f318-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-811">BatchAI</span></span>

* <span data-ttu-id="6f318-812">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="6f318-813">Cloud</span><span class="sxs-lookup"><span data-stu-id="6f318-813">Cloud</span></span>

* <span data-ttu-id="6f318-814">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="6f318-815">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-815">Container</span></span>

* <span data-ttu-id="6f318-816">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="6f318-817">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="6f318-818">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-819">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-819">Extension</span></span>

* <span data-ttu-id="6f318-820">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="6f318-821">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-821">Network</span></span>

* <span data-ttu-id="6f318-822">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="6f318-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6f318-823">Rdbms</span></span>

* <span data-ttu-id="6f318-824">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-825">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-825">Resource</span></span>

* <span data-ttu-id="6f318-826">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-827">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-827">VM</span></span>

* <span data-ttu-id="6f318-828">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="6f318-829">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-829">June 25, 2018</span></span>

<span data-ttu-id="6f318-830">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="6f318-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="6f318-831">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="6f318-831">CLI</span></span>

* <span data-ttu-id="6f318-832">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="6f318-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="6f318-833">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-833">June 19, 2018</span></span>

<span data-ttu-id="6f318-834">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="6f318-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="6f318-835">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-835">Core</span></span>

* <span data-ttu-id="6f318-836">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-837">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-837">ACR</span></span>

* <span data-ttu-id="6f318-838">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="6f318-839">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="6f318-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-840">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-840">ACS</span></span>

* <span data-ttu-id="6f318-841">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6f318-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="6f318-842">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-842">Added `--update` support</span></span>
* <span data-ttu-id="6f318-843">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="6f318-844">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="6f318-845">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="6f318-846">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="6f318-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="6f318-847">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="6f318-848">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-849">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-849">AppService</span></span>

* <span data-ttu-id="6f318-850">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="6f318-851">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-852">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-852">Batch</span></span>

* <span data-ttu-id="6f318-853">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6f318-854">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-854">Batch AI</span></span>

* <span data-ttu-id="6f318-855">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-855">Added support for workspaces.</span></span> <span data-ttu-id="6f318-856">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="6f318-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="6f318-857">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-857">Added support for experiments.</span></span> <span data-ttu-id="6f318-858">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="6f318-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="6f318-859">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="6f318-860">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="6f318-861">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="6f318-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="6f318-862">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="6f318-863">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="6f318-864">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="6f318-865">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="6f318-866">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="6f318-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="6f318-867">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="6f318-868">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="6f318-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="6f318-869">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="6f318-870">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="6f318-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="6f318-871">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="6f318-872">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="6f318-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="6f318-873">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="6f318-874">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6f318-875">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6f318-876">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="6f318-877">Karten</span><span class="sxs-lookup"><span data-stu-id="6f318-877">Maps</span></span>

* <span data-ttu-id="6f318-878">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="6f318-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="6f318-879">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-879">Network</span></span>

* <span data-ttu-id="6f318-880">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="6f318-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="6f318-881">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="6f318-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="6f318-882">#6502</span><span class="sxs-lookup"><span data-stu-id="6f318-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="6f318-883">Reservations</span><span class="sxs-lookup"><span data-stu-id="6f318-883">Reservations</span></span>

* <span data-ttu-id="6f318-884">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="6f318-885">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="6f318-886">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="6f318-887">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="6f318-888">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="6f318-889">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="6f318-890">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-890">Role</span></span>

* <span data-ttu-id="6f318-891">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-892">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-892">SQL</span></span>

* <span data-ttu-id="6f318-893">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="6f318-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-894">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-894">Storage</span></span>

* <span data-ttu-id="6f318-895">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-896">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-896">VM</span></span>

* <span data-ttu-id="6f318-897">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="6f318-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="6f318-898">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="6f318-899">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6f318-900">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-900">June 13, 2018</span></span>

<span data-ttu-id="6f318-901">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="6f318-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="6f318-902">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-902">Core</span></span>

* <span data-ttu-id="6f318-903">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="6f318-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6f318-904">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-904">June 13, 2018</span></span>

<span data-ttu-id="6f318-905">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="6f318-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="6f318-906">AKS</span><span class="sxs-lookup"><span data-stu-id="6f318-906">AKS</span></span>

* <span data-ttu-id="6f318-907">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="6f318-908">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="6f318-909">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="6f318-910">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="6f318-911">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-912">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-912">AppService</span></span>

* <span data-ttu-id="6f318-913">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6f318-914">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-914">June 5, 2018</span></span>

<span data-ttu-id="6f318-915">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="6f318-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-916">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-916">Interactive</span></span>

* <span data-ttu-id="6f318-917">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6f318-918">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-918">June 5, 2018</span></span>

<span data-ttu-id="6f318-919">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="6f318-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="6f318-920">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-920">Core</span></span>

* <span data-ttu-id="6f318-921">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="6f318-922">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="6f318-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-923">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-923">ACR</span></span>

* <span data-ttu-id="6f318-924">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="6f318-925">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="6f318-926">AKS</span><span class="sxs-lookup"><span data-stu-id="6f318-926">AKS</span></span>

* <span data-ttu-id="6f318-927">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f318-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-928">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-928">Batch</span></span>

* <span data-ttu-id="6f318-929">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="6f318-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-930">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-930">IOT</span></span>

* <span data-ttu-id="6f318-931">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="6f318-932">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-932">Network</span></span>

* <span data-ttu-id="6f318-933">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6f318-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6f318-934">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="6f318-934">Policy Insights</span></span>

* <span data-ttu-id="6f318-935">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="6f318-936">ARM</span><span class="sxs-lookup"><span data-stu-id="6f318-936">ARM</span></span>

* <span data-ttu-id="6f318-937">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-938">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-938">SQL</span></span>

* <span data-ttu-id="6f318-939">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="6f318-940">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="6f318-941">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-941">Storage</span></span>

* <span data-ttu-id="6f318-942">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="6f318-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-943">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-943">VM</span></span>

* <span data-ttu-id="6f318-944">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="6f318-945">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="6f318-946">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="6f318-947">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-947">May 22, 2018</span></span>

<span data-ttu-id="6f318-948">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="6f318-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="6f318-949">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-949">Core</span></span>

* <span data-ttu-id="6f318-950">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-951">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-951">ACS</span></span>

* <span data-ttu-id="6f318-952">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="6f318-953">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-954">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-954">AppService</span></span>

* <span data-ttu-id="6f318-955">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="6f318-955">Improved generic update commands</span></span>
* <span data-ttu-id="6f318-956">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="6f318-957">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-957">Container</span></span>

* <span data-ttu-id="6f318-958">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="6f318-959">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-960">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-960">Extension</span></span>

* <span data-ttu-id="6f318-961">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6f318-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-962">Interactive</span></span>

* <span data-ttu-id="6f318-963">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="6f318-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="6f318-964">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="6f318-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-965">KeyVault</span></span>

* <span data-ttu-id="6f318-966">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6f318-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="6f318-967">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-967">Network</span></span>

* <span data-ttu-id="6f318-968">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="6f318-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="6f318-969">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="6f318-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-970">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-970">SQL</span></span>

* <span data-ttu-id="6f318-971">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="6f318-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="6f318-972">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="6f318-973">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="6f318-974">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="6f318-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="6f318-975">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="6f318-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="6f318-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="6f318-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="6f318-977">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="6f318-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="6f318-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="6f318-978">`edition`.</span></span> <span data-ttu-id="6f318-979">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="6f318-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="6f318-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="6f318-980">`elasticPoolName`.</span></span> <span data-ttu-id="6f318-981">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="6f318-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="6f318-982">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="6f318-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="6f318-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="6f318-983">`edition`.</span></span> <span data-ttu-id="6f318-984">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="6f318-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="6f318-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="6f318-985">`dtu`.</span></span> <span data-ttu-id="6f318-986">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="6f318-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="6f318-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="6f318-987">`databaseDtuMin`.</span></span> <span data-ttu-id="6f318-988">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="6f318-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="6f318-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="6f318-989">`databaseDtuMax`.</span></span> <span data-ttu-id="6f318-990">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="6f318-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="6f318-991">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="6f318-992">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-993">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-993">Storage</span></span>

* <span data-ttu-id="6f318-994">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="6f318-995">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-996">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-996">VM</span></span>

* <span data-ttu-id="6f318-997">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="6f318-998">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="6f318-999">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="6f318-1000">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="6f318-1001">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="6f318-1002">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1002">May 7, 2018</span></span>

<span data-ttu-id="6f318-1003">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="6f318-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1004">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1004">Core</span></span>

* <span data-ttu-id="6f318-1005">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="6f318-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="6f318-1006">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="6f318-1007">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="6f318-1008">#5591</span><span class="sxs-lookup"><span data-stu-id="6f318-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="6f318-1009">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="6f318-1010">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="6f318-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="6f318-1011">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="6f318-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="6f318-1012">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="6f318-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="6f318-1013">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1014">ACR</span></span>

* <span data-ttu-id="6f318-1015">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="6f318-1016">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="6f318-1017">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="6f318-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="6f318-1018">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="6f318-1019">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="6f318-1020">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1021">ACS</span></span>

* <span data-ttu-id="6f318-1022">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="6f318-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="6f318-1023">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="6f318-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1024">AMS</span></span>

* <span data-ttu-id="6f318-1025">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6f318-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1026">Appservice</span></span>

* <span data-ttu-id="6f318-1027">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="6f318-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="6f318-1028">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="6f318-1029">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="6f318-1030">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6f318-1031">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-1031">Batch AI</span></span>

* <span data-ttu-id="6f318-1032">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6f318-1033">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6f318-1033">Cognitive Services</span></span>

* <span data-ttu-id="6f318-1034">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="6f318-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-1035">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-1035">Consumption</span></span>

* <span data-ttu-id="6f318-1036">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1037">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1037">Container</span></span>

* <span data-ttu-id="6f318-1038">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6f318-1039">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6f318-1039">Cosmos DB</span></span>

* <span data-ttu-id="6f318-1040">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6f318-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="6f318-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1041">DMS</span></span>

* <span data-ttu-id="6f318-1042">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1043">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1043">Extension</span></span>

* <span data-ttu-id="6f318-1044">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1045">Interactive</span></span>

* <span data-ttu-id="6f318-1046">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="6f318-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="6f318-1047">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="6f318-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="6f318-1048">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="6f318-1049">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="6f318-1050">Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-1050">Lab</span></span>

* <span data-ttu-id="6f318-1051">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1052">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1052">Network</span></span>

* <span data-ttu-id="6f318-1053">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="6f318-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="6f318-1054">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1054">Profile</span></span>

* <span data-ttu-id="6f318-1055">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="6f318-1056">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="6f318-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="6f318-1057">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="6f318-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="6f318-1058">Redis</span></span>

* <span data-ttu-id="6f318-1059">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="6f318-1060">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="6f318-1061">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="6f318-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="6f318-1062">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="6f318-1063">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1064">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1064">Role</span></span>

* <span data-ttu-id="6f318-1065">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1066">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1066">Storage</span></span>

* <span data-ttu-id="6f318-1067">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="6f318-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="6f318-1068">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="6f318-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="6f318-1069">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="6f318-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="6f318-1070">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="6f318-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="6f318-1071">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6f318-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1072">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1072">VM</span></span>

* <span data-ttu-id="6f318-1073">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="6f318-1074">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="6f318-1075">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="6f318-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="6f318-1076">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="6f318-1077">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="6f318-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="6f318-1078">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1078">Added write accelerator support</span></span>
* <span data-ttu-id="6f318-1079">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="6f318-1080">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="6f318-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="6f318-1081">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="6f318-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="6f318-1082">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1082">April 10, 2018</span></span>

<span data-ttu-id="6f318-1083">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="6f318-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1084">ACR</span></span>

* <span data-ttu-id="6f318-1085">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="6f318-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1086">ACS</span></span>

* <span data-ttu-id="6f318-1087">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1088">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1088">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="6f318-1090">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="6f318-1091">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6f318-1091">BatchAI</span></span>

* <span data-ttu-id="6f318-1092">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="6f318-1093">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="6f318-1093">Job level mounting</span></span>
  - <span data-ttu-id="6f318-1094">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="6f318-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="6f318-1095">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="6f318-1095">Performance counters settings</span></span>
  - <span data-ttu-id="6f318-1096">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="6f318-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="6f318-1097">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="6f318-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="6f318-1098">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="6f318-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="6f318-1099">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="6f318-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="6f318-1100">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="6f318-1100">Support for custom images</span></span>
  - <span data-ttu-id="6f318-1101">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="6f318-1102">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="6f318-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="6f318-1103">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="6f318-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="6f318-1104">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f318-1104">National clouds are supported</span></span>
* <span data-ttu-id="6f318-1105">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="6f318-1106">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="6f318-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="6f318-1107">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="6f318-1108">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="6f318-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="6f318-1109">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="6f318-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="6f318-1110">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="6f318-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="6f318-1111">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="6f318-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="6f318-1112">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="6f318-1113">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="6f318-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="6f318-1114">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="6f318-1115">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="6f318-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="6f318-1116">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="6f318-1117">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="6f318-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="6f318-1118">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="6f318-1118">Billing</span></span>

* <span data-ttu-id="6f318-1119">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-1120">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-1120">Consumption</span></span>

* <span data-ttu-id="6f318-1121">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="6f318-1122">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="6f318-1123">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="6f318-1124">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="6f318-1125">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="6f318-1126">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1127">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1127">Container</span></span>

* <span data-ttu-id="6f318-1128">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="6f318-1129">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1130">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1130">Extension</span></span>

* <span data-ttu-id="6f318-1131">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1132">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1132">Interactive</span></span>

* <span data-ttu-id="6f318-1133">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="6f318-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="6f318-1134">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="6f318-1135">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1136">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1136">Network</span></span>

* <span data-ttu-id="6f318-1137">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="6f318-1138">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="6f318-1139">#4910</span><span class="sxs-lookup"><span data-stu-id="6f318-1139">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="6f318-1140">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="6f318-1141">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="6f318-1142">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="6f318-1143">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="6f318-1144">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1145">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1145">Profile</span></span>

* <span data-ttu-id="6f318-1146">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="6f318-1147">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-1148">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1148">RDBMS</span></span>

* <span data-ttu-id="6f318-1149">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1149">Added `georestore` command</span></span>
* <span data-ttu-id="6f318-1150">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1151">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1151">Resource</span></span>

* <span data-ttu-id="6f318-1152">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="6f318-1153">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1154">SQL</span></span>

* <span data-ttu-id="6f318-1155">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1156">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1156">Storage</span></span>

* <span data-ttu-id="6f318-1157">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1158">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1158">VM</span></span>

* <span data-ttu-id="6f318-1159">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="6f318-1160">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="6f318-1162">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="6f318-1163">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="6f318-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="6f318-1164">#5718</span><span class="sxs-lookup"><span data-stu-id="6f318-1164">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="6f318-1165">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="6f318-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="6f318-1166">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1166">March 27, 2018</span></span>

<span data-ttu-id="6f318-1167">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="6f318-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1168">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1168">Core</span></span>

* <span data-ttu-id="6f318-1169">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="6f318-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1170">ACS</span></span>

* <span data-ttu-id="6f318-1171">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6f318-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1172">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1172">Appservice</span></span>

* <span data-ttu-id="6f318-1173">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="6f318-1174">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6f318-1175">Backup</span><span class="sxs-lookup"><span data-stu-id="6f318-1175">Backup</span></span>

* <span data-ttu-id="6f318-1176">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="6f318-1177">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="6f318-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="6f318-1178">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="6f318-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="6f318-1179">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="6f318-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1180">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1180">Container</span></span>

* <span data-ttu-id="6f318-1181">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1181">Added `container exec` command.</span></span> <span data-ttu-id="6f318-1182">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6f318-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="6f318-1183">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6f318-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1184">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1184">Extension</span></span>

* <span data-ttu-id="6f318-1185">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="6f318-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="6f318-1186">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="6f318-1187">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1188">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1188">Interactive</span></span>

* <span data-ttu-id="6f318-1189">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="6f318-1190">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="6f318-1191">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6f318-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="6f318-1192">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="6f318-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="6f318-1193">Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-1193">Lab</span></span>

* <span data-ttu-id="6f318-1194">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1195">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1195">Monitor</span></span>

* <span data-ttu-id="6f318-1196">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="6f318-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="6f318-1197">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="6f318-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="6f318-1198">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="6f318-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1199">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1199">Network</span></span>

* <span data-ttu-id="6f318-1200">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1201">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1201">Profile</span></span>

* <span data-ttu-id="6f318-1202">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-1203">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1203">RDBMS</span></span>

* <span data-ttu-id="6f318-1204">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1205">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1205">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="6f318-1207">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1207">Role</span></span>

* <span data-ttu-id="6f318-1208">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="6f318-1209">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6f318-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="6f318-1210">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="6f318-1211">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="6f318-1212">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1213">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1213">Storage</span></span>

* <span data-ttu-id="6f318-1214">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="6f318-1215">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="6f318-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1216">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1216">VM</span></span>

* <span data-ttu-id="6f318-1217">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="6f318-1218">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="6f318-1219">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="6f318-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="6f318-1220">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6f318-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="6f318-1221">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1221">March 13, 2018</span></span>

<span data-ttu-id="6f318-1222">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="6f318-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1223">ACR</span></span>

* <span data-ttu-id="6f318-1224">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="6f318-1225">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="6f318-1226">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1227">ACS</span></span>

* <span data-ttu-id="6f318-1228">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="6f318-1229">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="6f318-1230">Advisor</span><span class="sxs-lookup"><span data-stu-id="6f318-1230">Advisor</span></span>

* <span data-ttu-id="6f318-1231">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="6f318-1232">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="6f318-1233">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="6f318-1234">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="6f318-1235">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1236">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1236">Appservice</span></span>

* <span data-ttu-id="6f318-1237">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="6f318-1238">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="6f318-1239">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="6f318-1239">Eventhubs</span></span>

* <span data-ttu-id="6f318-1240">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1241">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1241">Extension</span></span>

* <span data-ttu-id="6f318-1242">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="6f318-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1243">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1243">Interactive</span></span>

* <span data-ttu-id="6f318-1244">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="6f318-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="6f318-1245">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="6f318-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="6f318-1246">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6f318-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="6f318-1247">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1248">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1248">Monitor</span></span>

* <span data-ttu-id="6f318-1249">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="6f318-1250">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="6f318-1251">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="6f318-1252">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1253">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1253">Network</span></span>

* <span data-ttu-id="6f318-1254">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="6f318-1255">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="6f318-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="6f318-1256">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="6f318-1257">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1258">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1258">Profile</span></span>

* <span data-ttu-id="6f318-1259">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="6f318-1260">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-1261">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1261">RDBMS</span></span>

* <span data-ttu-id="6f318-1262">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="6f318-1263">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6f318-1263">Service Bus</span></span>

* <span data-ttu-id="6f318-1264">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1265">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1265">Storage</span></span>

* <span data-ttu-id="6f318-1266">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="6f318-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="6f318-1267">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="6f318-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1268">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1268">VM</span></span>

* <span data-ttu-id="6f318-1269">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="6f318-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="6f318-1270">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="6f318-1271">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="6f318-1272">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="6f318-1273">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1273">February 27, 2018</span></span>

<span data-ttu-id="6f318-1274">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="6f318-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1275">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1275">Core</span></span>

* <span data-ttu-id="6f318-1276">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="6f318-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="6f318-1277">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="6f318-1278">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1279">ACS</span></span>

* <span data-ttu-id="6f318-1280">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="6f318-1281">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6f318-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="6f318-1282">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="6f318-1283">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1284">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1284">Appservice</span></span>

* <span data-ttu-id="6f318-1285">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="6f318-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="6f318-1286">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="6f318-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6f318-1287">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6f318-1287">Cognitive Services</span></span>

* <span data-ttu-id="6f318-1288">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-1289">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-1289">Consumption</span></span>

* <span data-ttu-id="6f318-1290">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="6f318-1291">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1292">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1292">Container</span></span>

* <span data-ttu-id="6f318-1293">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="6f318-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1294">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1294">Network</span></span>

* <span data-ttu-id="6f318-1295">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="6f318-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1296">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1296">Resource</span></span>

* <span data-ttu-id="6f318-1297">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="6f318-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1298">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1298">Role</span></span>

* <span data-ttu-id="6f318-1299">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1300">SQL</span></span>

* <span data-ttu-id="6f318-1301">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="6f318-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1302">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1302">Storage</span></span>

* <span data-ttu-id="6f318-1303">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1304">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1304">VM</span></span>

* <span data-ttu-id="6f318-1305">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="6f318-1306">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1306">February 13, 2018</span></span>

<span data-ttu-id="6f318-1307">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="6f318-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1308">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1308">Core</span></span>

* <span data-ttu-id="6f318-1309">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1310">ACS</span></span>

* <span data-ttu-id="6f318-1311">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="6f318-1312">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="6f318-1313">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="6f318-1314">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="6f318-1315">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="6f318-1316">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="6f318-1317">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6f318-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="6f318-1318">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="6f318-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1319">Appservice</span></span>

* <span data-ttu-id="6f318-1320">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="6f318-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="6f318-1321">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="6f318-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="6f318-1322">CDN</span></span>

* <span data-ttu-id="6f318-1323">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1324">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1324">Container</span></span>

* <span data-ttu-id="6f318-1325">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="6f318-1326">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-1327">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-1327">CosmosDB</span></span>

* <span data-ttu-id="6f318-1328">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1329">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1329">Extension</span></span>

* <span data-ttu-id="6f318-1330">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="6f318-1331">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="6f318-1332">Feedback</span><span class="sxs-lookup"><span data-stu-id="6f318-1332">Feedback</span></span>

* <span data-ttu-id="6f318-1333">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1334">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1334">Interactive</span></span>

* <span data-ttu-id="6f318-1335">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="6f318-1336">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-1337">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-1337">IoT</span></span>

* <span data-ttu-id="6f318-1338">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="6f318-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6f318-1339">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="6f318-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6f318-1340">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="6f318-1341">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1342">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1342">Monitor</span></span>

* <span data-ttu-id="6f318-1343">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1344">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1344">Network</span></span>

* <span data-ttu-id="6f318-1345">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="6f318-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="6f318-1346">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1346">Profile</span></span>

* <span data-ttu-id="6f318-1347">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="6f318-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1348">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1348">Resource</span></span>

* <span data-ttu-id="6f318-1349">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1350">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1350">Role</span></span>

* <span data-ttu-id="6f318-1351">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1352">SQL</span></span>

* <span data-ttu-id="6f318-1353">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="6f318-1354">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="6f318-1355">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1356">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1356">Storage</span></span>

* <span data-ttu-id="6f318-1357">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1358">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1358">VM</span></span>

* <span data-ttu-id="6f318-1359">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="6f318-1360">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="6f318-1361">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6f318-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="6f318-1362">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1362">January 31, 2018</span></span>

<span data-ttu-id="6f318-1363">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="6f318-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1364">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1364">Core</span></span>

* <span data-ttu-id="6f318-1365">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="6f318-1366">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="6f318-1367">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="6f318-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="6f318-1368">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f318-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="6f318-1369">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1370">ACS</span></span>

* <span data-ttu-id="6f318-1371">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="6f318-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="6f318-1372">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1373">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1373">Appservice</span></span>

* <span data-ttu-id="6f318-1374">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6f318-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="6f318-1375">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="6f318-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="6f318-1376">CDN</span></span>

* <span data-ttu-id="6f318-1377">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-1378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-1378">CosmosDB</span></span>

* <span data-ttu-id="6f318-1379">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1380">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1380">Interactive</span></span>

* <span data-ttu-id="6f318-1381">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1382">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1382">Network</span></span>

* <span data-ttu-id="6f318-1383">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="6f318-1384">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="6f318-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="6f318-1385">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="6f318-1386">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="6f318-1387">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="6f318-1388">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="6f318-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="6f318-1389">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="6f318-1390">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="6f318-1391">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="6f318-1392">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="6f318-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1393">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1393">Profile</span></span>

* <span data-ttu-id="6f318-1394">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1395">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1395">Resource</span></span>

* <span data-ttu-id="6f318-1396">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="6f318-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1397">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1397">Storage</span></span>

* <span data-ttu-id="6f318-1398">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="6f318-1399">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="6f318-1400">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6f318-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="6f318-1401">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="6f318-1402">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="6f318-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1403">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1403">VM</span></span>

* <span data-ttu-id="6f318-1404">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="6f318-1405">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="6f318-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="6f318-1406">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="6f318-1407">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="6f318-1408">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="6f318-1408">January 17, 2018</span></span>

<span data-ttu-id="6f318-1409">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="6f318-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1410">ACR</span></span>

* <span data-ttu-id="6f318-1411">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="6f318-1412">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="6f318-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1413">ACS</span></span>

* <span data-ttu-id="6f318-1414">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="6f318-1415">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1416">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1416">Appservice</span></span>

* <span data-ttu-id="6f318-1417">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="6f318-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="6f318-1418">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="6f318-1419">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="6f318-1420">Backup</span><span class="sxs-lookup"><span data-stu-id="6f318-1420">Backup</span></span>

* <span data-ttu-id="6f318-1421">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="6f318-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="6f318-1422">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="6f318-1423">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="6f318-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="6f318-1424">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="6f318-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="6f318-1425">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="6f318-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-1426">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-1426">Batch</span></span>

* <span data-ttu-id="6f318-1427">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6f318-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="6f318-1428">Cloud</span><span class="sxs-lookup"><span data-stu-id="6f318-1428">Cloud</span></span>

* <span data-ttu-id="6f318-1429">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-1430">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-1430">Consumption</span></span>

* <span data-ttu-id="6f318-1431">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="6f318-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="6f318-1432">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6f318-1432">Event Grid</span></span>

* <span data-ttu-id="6f318-1433">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6f318-1434">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6f318-1435">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="6f318-1436">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="6f318-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="6f318-1437">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="6f318-1438">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="6f318-1439">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="6f318-1440">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1441">Interactive</span><span class="sxs-lookup"><span data-stu-id="6f318-1441">Interactive</span></span>

* <span data-ttu-id="6f318-1442">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="6f318-1443">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="6f318-1444">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="6f318-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-1445">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-1445">IoT</span></span>

* <span data-ttu-id="6f318-1446">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="6f318-1447">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="6f318-1448">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="6f318-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1449">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1449">Monitor</span></span>

* <span data-ttu-id="6f318-1450">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="6f318-1451">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f318-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="6f318-1452">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1453">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1453">Network</span></span>

* <span data-ttu-id="6f318-1454">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="6f318-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="6f318-1455">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1456">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1456">Profile</span></span>

* <span data-ttu-id="6f318-1457">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1458">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1458">Role</span></span>

* <span data-ttu-id="6f318-1459">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="6f318-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6f318-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6f318-1460">Service Fabric</span></span>

* <span data-ttu-id="6f318-1461">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="6f318-1462">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1463">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1463">VM</span></span>

* <span data-ttu-id="6f318-1464">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="6f318-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="6f318-1465">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="6f318-1466">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="6f318-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="6f318-1467">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="6f318-1468">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="6f318-1469">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6f318-1470">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="6f318-1471">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="6f318-1472">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1472">December 19, 2017</span></span>

<span data-ttu-id="6f318-1473">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="6f318-1473">Version 2.0.23</span></span>

* <span data-ttu-id="6f318-1474">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1475">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1475">Container</span></span>

* <span data-ttu-id="6f318-1476">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1477">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1477">Network</span></span>

* <span data-ttu-id="6f318-1478">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="6f318-1479">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1480">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1480">Storage</span></span>

* <span data-ttu-id="6f318-1481">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1482">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1482">VM</span></span>

* <span data-ttu-id="6f318-1483">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="6f318-1484">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1484">December 5, 2017</span></span>

<span data-ttu-id="6f318-1485">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="6f318-1485">Version 2.0.22</span></span>

* <span data-ttu-id="6f318-1486">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1486">Removed `az component` commands.</span></span> <span data-ttu-id="6f318-1487">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="6f318-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1488">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1488">Core</span></span>
* <span data-ttu-id="6f318-1489">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="6f318-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="6f318-1490">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1491">ACS</span></span>

* <span data-ttu-id="6f318-1492">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="6f318-1493">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="6f318-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="6f318-1494">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="6f318-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="6f318-1495">Advisor</span><span class="sxs-lookup"><span data-stu-id="6f318-1495">Advisor</span></span>

* <span data-ttu-id="6f318-1496">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1497">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1497">Appservice</span></span>

* <span data-ttu-id="6f318-1498">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="6f318-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="6f318-1499">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6f318-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="6f318-1500">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="6f318-1501">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6f318-1501">Consumption</span></span>

* <span data-ttu-id="6f318-1502">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1503">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1503">Container</span></span>

* <span data-ttu-id="6f318-1504">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="6f318-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1505">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1505">Monitor</span></span>

* <span data-ttu-id="6f318-1506">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1507">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1507">Resource</span></span>

* <span data-ttu-id="6f318-1508">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1509">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1509">Role</span></span>

* <span data-ttu-id="6f318-1510">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="6f318-1511">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="6f318-1512">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6f318-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1513">SQL</span></span>

* <span data-ttu-id="6f318-1514">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="6f318-1515">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1516">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1516">VM</span></span>

* <span data-ttu-id="6f318-1517">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="6f318-1518">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1518">November 14, 2017</span></span>

<span data-ttu-id="6f318-1519">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="6f318-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1520">ACR</span></span>

* <span data-ttu-id="6f318-1521">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="6f318-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1522">ACS</span></span>

* <span data-ttu-id="6f318-1523">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="6f318-1524">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="6f318-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="6f318-1525">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="6f318-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="6f318-1526">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="6f318-1527">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1528">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1528">Appservice</span></span>

* <span data-ttu-id="6f318-1529">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="6f318-1530">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="6f318-1531">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="6f318-1532">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="6f318-1533">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="6f318-1534">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6f318-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-1535">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-1535">Batch</span></span>

* <span data-ttu-id="6f318-1536">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6f318-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="6f318-1537">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6f318-1537">Batchai</span></span>

* <span data-ttu-id="6f318-1538">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="6f318-1539">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="6f318-1540">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="6f318-1541">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="6f318-1542">Cloud</span><span class="sxs-lookup"><span data-stu-id="6f318-1542">Cloud</span></span>

* <span data-ttu-id="6f318-1543">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="6f318-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1544">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1544">Container</span></span>

* <span data-ttu-id="6f318-1545">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="6f318-1546">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1546">Added container group restart policy</span></span>
* <span data-ttu-id="6f318-1547">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="6f318-1548">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6f318-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6f318-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="6f318-1550">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="6f318-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6f318-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6f318-1551">Data Lake Store</span></span>

* <span data-ttu-id="6f318-1552">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="6f318-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1553">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1553">Extension</span></span>

* <span data-ttu-id="6f318-1554">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="6f318-1555">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6f318-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-1556">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-1556">IoT</span></span>

* <span data-ttu-id="6f318-1557">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1558">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1558">Monitor</span></span>

* <span data-ttu-id="6f318-1559">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1560">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1560">Network</span></span>

* <span data-ttu-id="6f318-1561">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="6f318-1562">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6f318-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="6f318-1563">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6f318-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="6f318-1564">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="6f318-1565">Reservations</span><span class="sxs-lookup"><span data-stu-id="6f318-1565">Reservations</span></span>

* <span data-ttu-id="6f318-1566">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6f318-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1567">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1567">Resource</span></span>

* <span data-ttu-id="6f318-1568">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1569">SQL</span></span>

* <span data-ttu-id="6f318-1570">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1571">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1571">Storage</span></span>

* <span data-ttu-id="6f318-1572">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="6f318-1573">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="6f318-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="6f318-1574">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6f318-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="6f318-1575">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="6f318-1576">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="6f318-1577">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="6f318-1578">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1579">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1579">VM</span></span>

* <span data-ttu-id="6f318-1580">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6f318-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="6f318-1581">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="6f318-1582">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="6f318-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="6f318-1583">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="6f318-1584">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="6f318-1585">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1585">October 24, 2017</span></span>

<span data-ttu-id="6f318-1586">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="6f318-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1587">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1587">Core</span></span>

* <span data-ttu-id="6f318-1588">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="6f318-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1589">ACR</span></span>

* <span data-ttu-id="6f318-1590">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="6f318-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="6f318-1591">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="6f318-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="6f318-1592">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1593">ACS</span></span>

* <span data-ttu-id="6f318-1594">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="6f318-1595">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1596">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1596">Appservice</span></span>

* <span data-ttu-id="6f318-1597">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="6f318-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="6f318-1598">Komponente</span><span class="sxs-lookup"><span data-stu-id="6f318-1598">Component</span></span>

* <span data-ttu-id="6f318-1599">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1600">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1600">Monitor</span></span>

* <span data-ttu-id="6f318-1601">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1602">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1602">Resource</span></span>

* <span data-ttu-id="6f318-1603">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="6f318-1604">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="6f318-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1605">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1605">VM</span></span>

* <span data-ttu-id="6f318-1606">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="6f318-1607">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1607">October 9, 2017</span></span>

<span data-ttu-id="6f318-1608">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="6f318-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1609">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1609">Core</span></span>

* <span data-ttu-id="6f318-1610">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1611">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1611">Appservice</span></span>

* <span data-ttu-id="6f318-1612">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-1613">Batch</span></span>

* <span data-ttu-id="6f318-1614">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="6f318-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="6f318-1615">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="6f318-1616">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="6f318-1617">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="6f318-1618">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6f318-1618">Batchai</span></span>

* <span data-ttu-id="6f318-1619">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-1620">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-1620">Keyvault</span></span>

* <span data-ttu-id="6f318-1621">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="6f318-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="6f318-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="6f318-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="6f318-1623">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1623">Network</span></span>

* <span data-ttu-id="6f318-1624">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="6f318-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="6f318-1625">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1626">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1626">Resource</span></span>

* <span data-ttu-id="6f318-1627">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="6f318-1628">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="6f318-1629">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="6f318-1630">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1631">Sql</span><span class="sxs-lookup"><span data-stu-id="6f318-1631">Sql</span></span>

* <span data-ttu-id="6f318-1632">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="6f318-1633">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="6f318-1634">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1635">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1635">Storage</span></span>

* <span data-ttu-id="6f318-1636">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1637">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1637">Vm</span></span>

* <span data-ttu-id="6f318-1638">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="6f318-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="6f318-1639">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="6f318-1640">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="6f318-1641">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="6f318-1642">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="6f318-1643">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1643">September 22, 2017</span></span>

<span data-ttu-id="6f318-1644">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="6f318-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1645">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1645">Resource</span></span>

* <span data-ttu-id="6f318-1646">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="6f318-1647">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="6f318-1648">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="6f318-1649">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="6f318-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1650">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1650">Network</span></span>

* <span data-ttu-id="6f318-1651">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="6f318-1652">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="6f318-1653">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="6f318-1654">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="6f318-1655">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6f318-1656">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="6f318-1657">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1658">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1658">Storage</span></span>

* <span data-ttu-id="6f318-1659">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6f318-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6f318-1660">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="6f318-1660">Eventgrid</span></span>

* <span data-ttu-id="6f318-1661">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1662">SQL</span></span>

* <span data-ttu-id="6f318-1663">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="6f318-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="6f318-1664">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f318-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="6f318-1665">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-1666">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-1666">Keyvault</span></span>

* <span data-ttu-id="6f318-1667">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1668">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1668">VM</span></span>

* <span data-ttu-id="6f318-1669">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="6f318-1670">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6f318-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="6f318-1671">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="6f318-1672">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="6f318-1673">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="6f318-1674">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1675">ACS</span></span>

* <span data-ttu-id="6f318-1676">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1677">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1677">Appservice</span></span>

* <span data-ttu-id="6f318-1678">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="6f318-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6f318-1679">Backup</span><span class="sxs-lookup"><span data-stu-id="6f318-1679">Backup</span></span>

* <span data-ttu-id="6f318-1680">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6f318-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="6f318-1681">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1681">September 11, 2017</span></span>

<span data-ttu-id="6f318-1682">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="6f318-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="6f318-1683">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1683">Core</span></span>

* <span data-ttu-id="6f318-1684">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="6f318-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="6f318-1685">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="6f318-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1686">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1686">Acs</span></span>

* <span data-ttu-id="6f318-1687">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="6f318-1688">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="6f318-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1689">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1689">Appservice</span></span>

* <span data-ttu-id="6f318-1690">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="6f318-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="6f318-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="6f318-1691">CDN</span></span>

* <span data-ttu-id="6f318-1692">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6f318-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="6f318-1693">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6f318-1693">Extension</span></span>

* <span data-ttu-id="6f318-1694">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-1695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-1695">Keyvault</span></span>

* <span data-ttu-id="6f318-1696">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="6f318-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1697">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1697">Network</span></span>

* <span data-ttu-id="6f318-1698">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6f318-1699">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="6f318-1700">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="6f318-1701">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6f318-1702">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1703">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1703">Resource</span></span>

* <span data-ttu-id="6f318-1704">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="6f318-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="6f318-1705">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="6f318-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="6f318-1706">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="6f318-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="6f318-1707">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1708">SQL</span></span>

* <span data-ttu-id="6f318-1709">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1710">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1710">VM</span></span>

* <span data-ttu-id="6f318-1711">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="6f318-1712">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="6f318-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="6f318-1713">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="6f318-1714">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="6f318-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="6f318-1715">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="6f318-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="6f318-1716">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1716">August 31, 2017</span></span>

<span data-ttu-id="6f318-1717">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="6f318-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-1718">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-1718">Keyvault</span></span>

* <span data-ttu-id="6f318-1719">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="6f318-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="6f318-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="6f318-1720">Sf</span></span>

* <span data-ttu-id="6f318-1721">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1722">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1722">Storage</span></span>

* <span data-ttu-id="6f318-1723">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="6f318-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="6f318-1724">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="6f318-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="6f318-1725">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1725">August 28, 2017</span></span>

<span data-ttu-id="6f318-1726">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="6f318-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="6f318-1727">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="6f318-1727">CLI</span></span>

* <span data-ttu-id="6f318-1728">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1729">ACS</span></span>

* <span data-ttu-id="6f318-1730">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1730">Corrected preview regions</span></span>
* <span data-ttu-id="6f318-1731">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="6f318-1732">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1733">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1733">Appservice</span></span>

* <span data-ttu-id="6f318-1734">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="6f318-1735">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="6f318-1736">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="6f318-1737">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="6f318-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="6f318-1738">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="6f318-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-1739">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-1739">IoT</span></span>

* <span data-ttu-id="6f318-1740">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6f318-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1741">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1741">Network</span></span>

* <span data-ttu-id="6f318-1742">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6f318-1743">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="6f318-1744">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6f318-1745">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6f318-1746">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1747">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1747">Profile</span></span>

* <span data-ttu-id="6f318-1748">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6f318-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6f318-1749">Service Fabric</span></span>

* <span data-ttu-id="6f318-1750">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6f318-1750">Preview release</span></span>
* <span data-ttu-id="6f318-1751">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="6f318-1752">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="6f318-1753">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1754">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1754">Storage</span></span>

* <span data-ttu-id="6f318-1755">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="6f318-1756">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="6f318-1757">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="6f318-1758">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="6f318-1759">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="6f318-1760">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="6f318-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1761">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1761">VM</span></span>

* <span data-ttu-id="6f318-1762">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="6f318-1763">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="6f318-1764">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="6f318-1765">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6f318-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="6f318-1766">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="6f318-1767">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="6f318-1768">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1768">August 15, 2017</span></span>

<span data-ttu-id="6f318-1769">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="6f318-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1770">ACS</span></span>

* <span data-ttu-id="6f318-1771">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1772">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1772">Appservice</span></span>

* <span data-ttu-id="6f318-1773">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="6f318-1774">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6f318-1774">Event Grid</span></span>

* <span data-ttu-id="6f318-1775">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="6f318-1776">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1776">August 11, 2017</span></span>

<span data-ttu-id="6f318-1777">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="6f318-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1778">ACS</span></span>

* <span data-ttu-id="6f318-1779">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-1780">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-1780">Batch</span></span>

* <span data-ttu-id="6f318-1781">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="6f318-1782">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="6f318-1783">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="6f318-1784">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="6f318-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="6f318-1785">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="6f318-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="6f318-1786">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="6f318-1787">Komponente</span><span class="sxs-lookup"><span data-stu-id="6f318-1787">Component</span></span>

* <span data-ttu-id="6f318-1788">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="6f318-1789">Container</span><span class="sxs-lookup"><span data-stu-id="6f318-1789">Container</span></span>

* <span data-ttu-id="6f318-1790">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="6f318-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="6f318-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6f318-1791">Data Lake Store</span></span>

* <span data-ttu-id="6f318-1792">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="6f318-1793">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6f318-1793">Event Grid</span></span>

* <span data-ttu-id="6f318-1794">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6f318-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1795">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1795">Network</span></span>

* <span data-ttu-id="6f318-1796">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="6f318-1797">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="6f318-1798">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="6f318-1799">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="6f318-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1800">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1800">Profile</span></span>

* <span data-ttu-id="6f318-1801">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="6f318-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1802">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1802">Storage</span></span>

* <span data-ttu-id="6f318-1803">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1804">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1804">VM</span></span>

* <span data-ttu-id="6f318-1805">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="6f318-1806">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="6f318-1807">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="6f318-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="6f318-1808">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="6f318-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="6f318-1809">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="6f318-1810">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1810">July 28, 2017</span></span>

<span data-ttu-id="6f318-1811">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="6f318-1811">Version 2.0.12</span></span>

* <span data-ttu-id="6f318-1812">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1812">Added container commands</span></span>
* <span data-ttu-id="6f318-1813">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="6f318-1814">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-1814">Core</span></span>

* <span data-ttu-id="6f318-1815">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="6f318-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="6f318-1816">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="6f318-1817">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="6f318-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="6f318-1818">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="6f318-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="6f318-1819">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="6f318-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="6f318-1820">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="6f318-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="6f318-1821">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6f318-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6f318-1822">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="6f318-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="6f318-1823">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="6f318-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="6f318-1824">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="6f318-1825">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="6f318-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="6f318-1826">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="6f318-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="6f318-1827">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6f318-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="6f318-1828">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6f318-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="6f318-1829">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6f318-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="6f318-1830">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="6f318-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="6f318-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1831">ACR</span></span>

* <span data-ttu-id="6f318-1832">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="6f318-1833">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="6f318-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="6f318-1834">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="6f318-1835">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="6f318-1836">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="6f318-1837">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-1838">ACS</span></span>

* <span data-ttu-id="6f318-1839">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="6f318-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-1840">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-1840">Appservice</span></span>

* <span data-ttu-id="6f318-1841">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="6f318-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="6f318-1842">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="6f318-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="6f318-1843">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="6f318-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="6f318-1844">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="6f318-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="6f318-1845">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="6f318-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="6f318-1846">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="6f318-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="6f318-1847">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="6f318-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="6f318-1848">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="6f318-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="6f318-1849">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="6f318-1850">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="6f318-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="6f318-1851">Batch</span><span class="sxs-lookup"><span data-stu-id="6f318-1851">Batch</span></span>

* <span data-ttu-id="6f318-1852">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="6f318-1853">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="6f318-1854">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="6f318-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="6f318-1855">CDN</span></span>

* <span data-ttu-id="6f318-1856">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6f318-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="6f318-1857">Cloud</span><span class="sxs-lookup"><span data-stu-id="6f318-1857">Cloud</span></span>

* <span data-ttu-id="6f318-1858">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="6f318-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="6f318-1859">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f318-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="6f318-1860">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="6f318-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="6f318-1861">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="6f318-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="6f318-1862">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6f318-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-1863">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-1863">CosmosDB</span></span>

* <span data-ttu-id="6f318-1864">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="6f318-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="6f318-1865">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6f318-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6f318-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="6f318-1867">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="6f318-1868">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="6f318-1869">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6f318-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6f318-1870">Data Lake Store</span></span>

* <span data-ttu-id="6f318-1871">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="6f318-1872">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6f318-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="6f318-1873">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="6f318-1874">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6f318-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="6f318-1875">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="6f318-1875">Interactive</span></span>

* <span data-ttu-id="6f318-1876">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="6f318-1877">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1877">Increased test coverage</span></span>
* <span data-ttu-id="6f318-1878">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="6f318-1879">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="6f318-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="6f318-1880">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="6f318-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="6f318-1881">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="6f318-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="6f318-1882">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6f318-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6f318-1883">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="6f318-1884">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="6f318-1885">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="6f318-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="6f318-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="6f318-1886">IoT</span></span>

* <span data-ttu-id="6f318-1887">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6f318-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="6f318-1888">(3934)</span><span class="sxs-lookup"><span data-stu-id="6f318-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="6f318-1889">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="6f318-1889">Key vault</span></span>

* <span data-ttu-id="6f318-1890">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6f318-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="6f318-1891">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6f318-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="6f318-1892">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6f318-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6f318-1893">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6f318-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6f318-1894">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6f318-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="6f318-1895">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="6f318-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="6f318-1896">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="6f318-1897">(3307)</span><span class="sxs-lookup"><span data-stu-id="6f318-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="6f318-1898">Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-1898">Lab</span></span>

* <span data-ttu-id="6f318-1899">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="6f318-1900">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-1901">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-1901">Monitor</span></span>

* <span data-ttu-id="6f318-1902">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="6f318-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="6f318-1903">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="6f318-1904">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="6f318-1905">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="6f318-1906">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6f318-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="6f318-1907">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="6f318-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="6f318-1908">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="6f318-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="6f318-1909">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="6f318-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="6f318-1910">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f318-1910">`location` no longer required</span></span>
  * <span data-ttu-id="6f318-1911">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="6f318-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="6f318-1912">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="6f318-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="6f318-1913">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="6f318-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="6f318-1914">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6f318-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="6f318-1915">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="6f318-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="6f318-1916">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="6f318-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="6f318-1917">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="6f318-1918">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-1918">Network</span></span>

* <span data-ttu-id="6f318-1919">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="6f318-1920">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="6f318-1921">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6f318-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="6f318-1922">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6f318-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="6f318-1923">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6f318-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="6f318-1924">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="6f318-1925">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="6f318-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="6f318-1926">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="6f318-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="6f318-1927">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="6f318-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="6f318-1928">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="6f318-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="6f318-1929">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="6f318-1930">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="6f318-1931">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="6f318-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="6f318-1932">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="6f318-1933">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="6f318-1934">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="6f318-1935">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="6f318-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="6f318-1936">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="6f318-1937">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="6f318-1938">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="6f318-1939">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="6f318-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="6f318-1940">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6f318-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="6f318-1941">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="6f318-1942">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6f318-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="6f318-1943">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6f318-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="6f318-1944">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6f318-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="6f318-1945">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6f318-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-1946">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-1946">Profile</span></span>

* <span data-ttu-id="6f318-1947">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="6f318-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="6f318-1948">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="6f318-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="6f318-1949">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="6f318-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="6f318-1950">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="6f318-1951">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="6f318-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="6f318-1952">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6f318-1952">RDBMS</span></span>

* <span data-ttu-id="6f318-1953">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="6f318-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="6f318-1954">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="6f318-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="6f318-1955">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="6f318-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="6f318-1956">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="6f318-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-1957">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-1957">Resource</span></span>

* <span data-ttu-id="6f318-1958">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="6f318-1959">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="6f318-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="6f318-1960">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="6f318-1961">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="6f318-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="6f318-1962">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="6f318-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="6f318-1963">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="6f318-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="6f318-1964">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="6f318-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="6f318-1965">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="6f318-1966">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-1966">Role</span></span>

* <span data-ttu-id="6f318-1967">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6f318-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="6f318-1968">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="6f318-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="6f318-1969">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="6f318-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="6f318-1970">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="6f318-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="6f318-1971">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6f318-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6f318-1972">Service Fabric</span></span>
* <span data-ttu-id="6f318-1973">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="6f318-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="6f318-1974">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="6f318-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="6f318-1975">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="6f318-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-1976">SQL</span></span>

* <span data-ttu-id="6f318-1977">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="6f318-1978">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6f318-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="6f318-1979">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-1980">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-1980">Storage</span></span>

* <span data-ttu-id="6f318-1981">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="6f318-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="6f318-1982">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6f318-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="6f318-1983">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="6f318-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="6f318-1984">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="6f318-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="6f318-1985">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="6f318-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="6f318-1986">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="6f318-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-1987">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-1987">VM</span></span>

* <span data-ttu-id="6f318-1988">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="6f318-1988">Support configuring nsg</span></span>
* <span data-ttu-id="6f318-1989">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="6f318-1990">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="6f318-1990">Support managed service identities</span></span>
* <span data-ttu-id="6f318-1991">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="6f318-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="6f318-1992">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="6f318-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="6f318-1993">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-1993">May 10, 2017</span></span>

<span data-ttu-id="6f318-1994">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="6f318-1994">Version 2.0.6</span></span>

* <span data-ttu-id="6f318-1995">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="6f318-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="6f318-1996">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="6f318-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="6f318-1997">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="6f318-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="6f318-1998">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="6f318-1999">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="6f318-2000">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="6f318-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="6f318-2001">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="6f318-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="6f318-2002">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="6f318-2002">Remove Container module</span></span>
* <span data-ttu-id="6f318-2003">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="6f318-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="6f318-2004">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6f318-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="6f318-2005">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-2005">Core</span></span>

* <span data-ttu-id="6f318-2006">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="6f318-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="6f318-2007">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="6f318-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="6f318-2008">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="6f318-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="6f318-2009">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="6f318-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="6f318-2010">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="6f318-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="6f318-2011">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="6f318-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="6f318-2012">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="6f318-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="6f318-2013">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="6f318-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="6f318-2014">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="6f318-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="6f318-2015">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="6f318-2015">core: Improved performance</span></span>
* <span data-ttu-id="6f318-2016">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="6f318-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="6f318-2017">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="6f318-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-2018">ACS</span></span>

* <span data-ttu-id="6f318-2019">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f318-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="6f318-2020">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="6f318-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="6f318-2021">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="6f318-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="6f318-2022">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="6f318-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-2023">AppService</span></span>

* <span data-ttu-id="6f318-2024">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="6f318-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="6f318-2025">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="6f318-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="6f318-2026">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="6f318-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="6f318-2027">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="6f318-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="6f318-2028">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="6f318-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="6f318-2029">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="6f318-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="6f318-2030">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="6f318-2030">support slot swap with preview</span></span>
* <span data-ttu-id="6f318-2031">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="6f318-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="6f318-2032">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="6f318-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6f318-2033">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6f318-2033">CosmosDB</span></span>

* <span data-ttu-id="6f318-2034">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="6f318-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="6f318-2035">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="6f318-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="6f318-2036">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="6f318-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="6f318-2037">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="6f318-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6f318-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6f318-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="6f318-2039">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="6f318-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="6f318-2040">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="6f318-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="6f318-2041">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="6f318-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="6f318-2042">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="6f318-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="6f318-2043">Table</span><span class="sxs-lookup"><span data-stu-id="6f318-2043">Table</span></span>
  * <span data-ttu-id="6f318-2044">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="6f318-2044">Table valued function</span></span>
  * <span data-ttu-id="6f318-2045">Sicht</span><span class="sxs-lookup"><span data-stu-id="6f318-2045">View</span></span>
  * <span data-ttu-id="6f318-2046">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="6f318-2046">Table Statistics.</span></span> <span data-ttu-id="6f318-2047">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="6f318-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6f318-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6f318-2048">Data Lake Store</span></span>

* <span data-ttu-id="6f318-2049">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="6f318-2050">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6f318-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="6f318-2051">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="6f318-2051">missed help for access show.</span></span> <span data-ttu-id="6f318-2052">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6f318-2052">adding it.</span></span> <span data-ttu-id="6f318-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="6f318-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="6f318-2054">Suchen</span><span class="sxs-lookup"><span data-stu-id="6f318-2054">Find</span></span>

* <span data-ttu-id="6f318-2055">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="6f318-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f318-2056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f318-2056">KeyVault</span></span>

* <span data-ttu-id="6f318-2057">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="6f318-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="6f318-2058">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="6f318-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="6f318-2059">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="6f318-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="6f318-2060">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="6f318-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="6f318-2061">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="6f318-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="6f318-2062">Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-2062">Lab</span></span>

* <span data-ttu-id="6f318-2063">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="6f318-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="6f318-2064">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="6f318-2065">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="6f318-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="6f318-2066">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="6f318-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="6f318-2067">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="6f318-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="6f318-2068">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6f318-2068">Monitor</span></span>

* <span data-ttu-id="6f318-2069">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="6f318-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="6f318-2070">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="6f318-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="6f318-2071">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-2071">Network</span></span>

* <span data-ttu-id="6f318-2072">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="6f318-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="6f318-2073">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="6f318-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="6f318-2074">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="6f318-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="6f318-2075">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="6f318-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="6f318-2076">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="6f318-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="6f318-2077">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="6f318-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="6f318-2078">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6f318-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="6f318-2079">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6f318-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="6f318-2080">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="6f318-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="6f318-2081">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="6f318-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="6f318-2082">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="6f318-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="6f318-2083">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="6f318-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="6f318-2084">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="6f318-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="6f318-2085">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6f318-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="6f318-2086">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6f318-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="6f318-2087">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="6f318-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="6f318-2088">Profil</span><span class="sxs-lookup"><span data-stu-id="6f318-2088">Profile</span></span>

* <span data-ttu-id="6f318-2089">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="6f318-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="6f318-2090">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="6f318-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="6f318-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="6f318-2091">Redis</span></span>

* <span data-ttu-id="6f318-2092">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="6f318-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="6f318-2093">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="6f318-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="6f318-2094">Ressource</span><span class="sxs-lookup"><span data-stu-id="6f318-2094">Resource</span></span>

* <span data-ttu-id="6f318-2095">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="6f318-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="6f318-2096">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="6f318-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="6f318-2097">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="6f318-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="6f318-2098">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="6f318-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="6f318-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="6f318-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="6f318-2100">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="6f318-2100">Add docs for az lock update.</span></span> <span data-ttu-id="6f318-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="6f318-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="6f318-2102">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="6f318-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="6f318-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="6f318-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="6f318-2104">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="6f318-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="6f318-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="6f318-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="6f318-2106">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="6f318-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="6f318-2107">Rolle</span><span class="sxs-lookup"><span data-stu-id="6f318-2107">Role</span></span>

* <span data-ttu-id="6f318-2108">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="6f318-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="6f318-2109">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="6f318-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="6f318-2110">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="6f318-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="6f318-2111">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="6f318-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="6f318-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="6f318-2112">SQL</span></span>

* <span data-ttu-id="6f318-2113">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="6f318-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="6f318-2114">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="6f318-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="6f318-2115">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-2115">Storage</span></span>

* <span data-ttu-id="6f318-2116">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="6f318-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="6f318-2117">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="6f318-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="6f318-2118">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="6f318-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="6f318-2119">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="6f318-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-2120">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-2120">VM</span></span>

* <span data-ttu-id="6f318-2121">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="6f318-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="6f318-2122">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="6f318-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="6f318-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="6f318-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="6f318-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="6f318-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="6f318-2125">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="6f318-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="6f318-2126">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="6f318-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="6f318-2127">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="6f318-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="6f318-2128">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-2128">April 3, 2017</span></span>

<span data-ttu-id="6f318-2129">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="6f318-2129">Version 2.0.2</span></span>

<span data-ttu-id="6f318-2130">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="6f318-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="6f318-2131">Core</span><span class="sxs-lookup"><span data-stu-id="6f318-2131">Core</span></span>

* <span data-ttu-id="6f318-2132">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="6f318-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="6f318-2133">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="6f318-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="6f318-2134">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="6f318-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="6f318-2135">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6f318-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6f318-2136">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="6f318-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="6f318-2137">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="6f318-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="6f318-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="6f318-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="6f318-2139">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="6f318-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="6f318-2140">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="6f318-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="6f318-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="6f318-2141">ACS</span></span>

* <span data-ttu-id="6f318-2142">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="6f318-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="6f318-2143">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="6f318-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="6f318-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="6f318-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="6f318-2145">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="6f318-2145">Add support for windows clusters.</span></span> <span data-ttu-id="6f318-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="6f318-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="6f318-2147">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="6f318-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="6f318-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="6f318-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="6f318-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="6f318-2149">AppService</span></span>

* <span data-ttu-id="6f318-2150">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="6f318-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="6f318-2151">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="6f318-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="6f318-2152">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="6f318-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="6f318-2153">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="6f318-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="6f318-2154">DataLake</span><span class="sxs-lookup"><span data-stu-id="6f318-2154">DataLake</span></span>

* <span data-ttu-id="6f318-2155">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="6f318-2156">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="6f318-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="6f318-2157">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="6f318-2157">DocuemntDB</span></span>

* <span data-ttu-id="6f318-2158">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="6f318-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="6f318-2159">VM</span><span class="sxs-lookup"><span data-stu-id="6f318-2159">VM</span></span>

* <span data-ttu-id="6f318-2160">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="6f318-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="6f318-2161">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="6f318-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="6f318-2162">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="6f318-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="6f318-2163">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6f318-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6f318-2164">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="6f318-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="6f318-2165">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="6f318-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="6f318-2166">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="6f318-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="6f318-2167">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="6f318-2167">February 27, 2017</span></span>

<span data-ttu-id="6f318-2168">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="6f318-2168">Version 2.0.0</span></span>

<span data-ttu-id="6f318-2169">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="6f318-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="6f318-2170">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="6f318-2170">Container Service (acs)</span></span>
- <span data-ttu-id="6f318-2171">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="6f318-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="6f318-2172">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6f318-2172">Networking</span></span>
- <span data-ttu-id="6f318-2173">Storage</span><span class="sxs-lookup"><span data-stu-id="6f318-2173">Storage</span></span>

<span data-ttu-id="6f318-2174">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="6f318-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="6f318-2175">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="6f318-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="6f318-2176">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="6f318-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="6f318-2177">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="6f318-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="6f318-2178">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="6f318-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="6f318-2179">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="6f318-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="6f318-2180">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="6f318-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="6f318-2181">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="6f318-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="6f318-2182">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="6f318-2182">Provide feedback from the command line with the `az feedback` command</span></span>


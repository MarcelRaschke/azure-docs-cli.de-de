---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8307ca9797a9a780d7e08d6d21cb66446c7e289
ms.sourcegitcommit: 6d9e8ee6dd07cfd07239a2948304d7f50ef781cc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "58508901"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="96718-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="96718-103">Azure CLI release notes</span></span>
## <a name="march-26-2019"></a><span data-ttu-id="96718-104">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="96718-104">March 26, 2019</span></span>

### <a name="core"></a><span data-ttu-id="96718-105">Core</span><span class="sxs-lookup"><span data-stu-id="96718-105">Core</span></span>
* <span data-ttu-id="96718-106">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="96718-106">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="96718-107">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="96718-107">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="96718-108">Cloud</span><span class="sxs-lookup"><span data-stu-id="96718-108">Cloud</span></span>
* <span data-ttu-id="96718-109">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-109">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="96718-110">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-110">ACR</span></span>
* <span data-ttu-id="96718-111">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-111">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="96718-112">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-112">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="96718-113">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-113">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="96718-114">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-114">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-115">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-115">AppService</span></span>
* <span data-ttu-id="96718-116">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="96718-116">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="96718-117">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="96718-117">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="96718-118">Bot Service</span><span class="sxs-lookup"><span data-stu-id="96718-118">BOT Service</span></span>
* <span data-ttu-id="96718-119">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="96718-119">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="96718-120">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="96718-120">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="96718-121">[BREAKING CHANGE] `--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="96718-121">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="96718-122">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-122">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-123">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-123">CDN</span></span>
* <span data-ttu-id="96718-124">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-124">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="96718-125">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="96718-125">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="96718-126">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="96718-126">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="96718-127">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="96718-127">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-128">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="96718-128">Cosmosdb</span></span>
* <span data-ttu-id="96718-129">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-129">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="96718-130">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-130">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-131">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-131">Interactive</span></span>
* <span data-ttu-id="96718-132">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-132">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-133">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-133">Monitor</span></span>
* <span data-ttu-id="96718-134">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="96718-134">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="96718-135">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-135">Network</span></span>
* <span data-ttu-id="96718-136">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-136">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-137">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-137">Profile</span></span>
* <span data-ttu-id="96718-138">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-138">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="96718-139">Postgres</span><span class="sxs-lookup"><span data-stu-id="96718-139">Postgres</span></span> 
* <span data-ttu-id="96718-140">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-140">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="96718-141">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="96718-141">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="96718-142">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-142">Resource</span></span>
* <span data-ttu-id="96718-143">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="96718-143">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="96718-144">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="96718-144">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="96718-145">Graph</span><span class="sxs-lookup"><span data-stu-id="96718-145">Graph</span></span>
* <span data-ttu-id="96718-146">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-146">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="96718-147">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-147">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="96718-148">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="96718-148">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="96718-149">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="96718-149">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="96718-150">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-150">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="96718-151">storage</span><span class="sxs-lookup"><span data-stu-id="96718-151">storage</span></span>
* <span data-ttu-id="96718-152">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-152">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="96718-153">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="96718-153">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="96718-154">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="96718-154">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="96718-155">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="96718-155">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="96718-156">VM</span><span class="sxs-lookup"><span data-stu-id="96718-156">VM</span></span>
* <span data-ttu-id="96718-157">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-157">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="96718-158">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="96718-158">March 12, 2019</span></span>

<span data-ttu-id="96718-159">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="96718-159">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="96718-160">Core</span><span class="sxs-lookup"><span data-stu-id="96718-160">Core</span></span>

* <span data-ttu-id="96718-161">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-161">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="96718-162">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-162">ACR</span></span>

* <span data-ttu-id="96718-163">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-163">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="96718-164">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-164">ACS</span></span>

* <span data-ttu-id="96718-165">Geändert, sodass das Argument `--listen-address` für `aks browse` ignoriert wird, wenn es von `kubectl` nicht unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="96718-165">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-166">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-166">AppService</span></span>

* <span data-ttu-id="96718-167">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="96718-167">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="96718-168">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-168">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="96718-169">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="96718-169">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="96718-170">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="96718-170">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="96718-171">Botservice</span><span class="sxs-lookup"><span data-stu-id="96718-171">Botservice</span></span>

* <span data-ttu-id="96718-172">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-172">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="96718-173">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-173">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="96718-174">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-174">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="96718-175">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="96718-175">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="96718-176">Container</span><span class="sxs-lookup"><span data-stu-id="96718-176">Container</span></span>

* <span data-ttu-id="96718-177">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-177">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="96718-178">EventHub</span><span class="sxs-lookup"><span data-stu-id="96718-178">EventHub</span></span>

* <span data-ttu-id="96718-179">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-179">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="96718-180">Suchen</span><span class="sxs-lookup"><span data-stu-id="96718-180">Find</span></span>

* <span data-ttu-id="96718-181">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="96718-181">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="96718-182">HDInsight</span><span class="sxs-lookup"><span data-stu-id="96718-182">HDInsight</span></span>

* <span data-ttu-id="96718-183">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-183">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="96718-184">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-184">Network</span></span>

* <span data-ttu-id="96718-185">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="96718-185">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-186">Rdbms</span><span class="sxs-lookup"><span data-stu-id="96718-186">Rdbms</span></span>

* <span data-ttu-id="96718-187">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="96718-187">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="96718-188">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-188">Role</span></span>

* <span data-ttu-id="96718-189">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="96718-189">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="96718-190">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="96718-190">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="96718-191">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="96718-191">Service Fabric</span></span>

* <span data-ttu-id="96718-192">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-192">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="96718-193">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="96718-193">February 26, 2019</span></span>

<span data-ttu-id="96718-194">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="96718-194">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="96718-195">Core</span><span class="sxs-lookup"><span data-stu-id="96718-195">Core</span></span>

* <span data-ttu-id="96718-196">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="96718-196">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="96718-197">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-197">ACR</span></span>

* <span data-ttu-id="96718-198">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-198">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="96718-199">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="96718-199">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="96718-200">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-200">ACS</span></span>

* <span data-ttu-id="96718-201">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-201">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-202">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-202">AppService</span></span>

* <span data-ttu-id="96718-203">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-203">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="96718-204">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-204">Batch</span></span>
* <span data-ttu-id="96718-205">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-205">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="96718-206">[BREAKING CHANGE] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-206">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="96718-207">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-207">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="96718-208">[BREAKING CHANGE] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="96718-208">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="96718-209">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-209">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="96718-210">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="96718-210">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-211">CosmosDB</span></span>

* <span data-ttu-id="96718-212">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-212">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="96718-213">Kusto</span><span class="sxs-lookup"><span data-stu-id="96718-213">Kusto</span></span>

* <span data-ttu-id="96718-214">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="96718-214">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="96718-215">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-215">Network</span></span>

* <span data-ttu-id="96718-216">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-216">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="96718-217">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-217">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="96718-218">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-218">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="96718-219">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-219">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="96718-220">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-220">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="96718-221">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-221">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="96718-222">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-222">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="96718-223">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-223">Resource</span></span>

* <span data-ttu-id="96718-224">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="96718-224">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="96718-225">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-225">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="96718-226">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-226">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="96718-227">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-227">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="96718-228">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="96718-228">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="96718-229">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-229">Role</span></span>

* <span data-ttu-id="96718-230">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-230">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-231">VM</span><span class="sxs-lookup"><span data-stu-id="96718-231">VM</span></span>

* <span data-ttu-id="96718-232">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="96718-232">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="96718-233">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="96718-233">February 12, 2019</span></span>

<span data-ttu-id="96718-234">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="96718-234">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="96718-235">Core</span><span class="sxs-lookup"><span data-stu-id="96718-235">Core</span></span>

* <span data-ttu-id="96718-236">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="96718-236">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="96718-237">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-237">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="96718-238">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-238">ACR</span></span>
* <span data-ttu-id="96718-239">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-239">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="96718-240">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-240">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="96718-241">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-241">ACS</span></span>
* <span data-ttu-id="96718-242">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-242">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="96718-243">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-243">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="96718-244">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-244">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="96718-245">AMS</span><span class="sxs-lookup"><span data-stu-id="96718-245">AMS</span></span>
* <span data-ttu-id="96718-246">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-246">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="96718-247">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-247">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-248">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-248">Appservice</span></span>
* <span data-ttu-id="96718-249">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-249">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="96718-250">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-250">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="96718-251">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="96718-251">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="96718-252">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-252">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="96718-253">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-253">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="96718-254">Botservice</span><span class="sxs-lookup"><span data-stu-id="96718-254">Botservice</span></span>
* <span data-ttu-id="96718-255">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="96718-255">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="96718-256">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-256">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="96718-257">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-257">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="96718-258">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="96718-258">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="96718-259">[VERALTET] Das `--proj-name`-Argument wurde zugunsten von `--proj-file-path` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="96718-259">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="96718-260">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="96718-260">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="96718-261">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="96718-261">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="96718-262">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-262">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="96718-263">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="96718-263">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="96718-264">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="96718-264">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="96718-265">Key Vault</span><span class="sxs-lookup"><span data-stu-id="96718-265">Key Vault</span></span>
* <span data-ttu-id="96718-266">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="96718-266">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-267">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-267">Monitor</span></span>
* <span data-ttu-id="96718-268">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="96718-268">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="96718-269">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-269">Network</span></span>
* <span data-ttu-id="96718-270">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="96718-270">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="96718-271">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="96718-271">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="96718-272">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="96718-272">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="96718-273">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-273">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="96718-274">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="96718-274">Policy Insights</span></span>
* <span data-ttu-id="96718-275">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="96718-275">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-276">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-276">RDBMS</span></span>
* <span data-ttu-id="96718-277">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="96718-277">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="96718-278">Redis</span><span class="sxs-lookup"><span data-stu-id="96718-278">Redis</span></span>
* <span data-ttu-id="96718-279">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-279">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="96718-280">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-280">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="96718-281">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-281">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="96718-282">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-282">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="96718-283">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-283">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="96718-284">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="96718-284">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="96718-285">[VERALTET] Warnmeldung für die Deaktivierung von des Befehls `redis import-method` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-285">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="96718-286">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-286">Role</span></span>
* <span data-ttu-id="96718-287">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="96718-287">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="96718-288">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="96718-288">SQL VM</span></span>
* <span data-ttu-id="96718-289">[VERALTET] Das `--boostrap-acc-pwd`-Argument wurde aufgrund eines Tippfehlers als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="96718-289">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="96718-290">VM</span><span class="sxs-lookup"><span data-stu-id="96718-290">VM</span></span>
* <span data-ttu-id="96718-291">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="96718-291">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="96718-292">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-292">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="96718-293">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="96718-293">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="96718-294">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="96718-294">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="96718-295">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="96718-295">January 31, 2019</span></span>

<span data-ttu-id="96718-296">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="96718-296">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="96718-297">Core</span><span class="sxs-lookup"><span data-stu-id="96718-297">Core</span></span>

* <span data-ttu-id="96718-298">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="96718-298">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="96718-299">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="96718-299">January 28, 2019</span></span>

<span data-ttu-id="96718-300">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="96718-300">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="96718-301">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-301">ACR</span></span>
* <span data-ttu-id="96718-302">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-302">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="96718-303">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-303">ACS</span></span>
* <span data-ttu-id="96718-304">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-304">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="96718-305">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-305">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="96718-306">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-306">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="96718-307">AMS</span><span class="sxs-lookup"><span data-stu-id="96718-307">AMS</span></span>
* <span data-ttu-id="96718-308">[BREAKING CHANGE] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-308">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="96718-309">[BREAKING CHANGE] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-309">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-310">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-310">Appservice</span></span>
* <span data-ttu-id="96718-311">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-311">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="96718-312">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-312">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="96718-313">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-313">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="96718-314">Container</span><span class="sxs-lookup"><span data-stu-id="96718-314">Container</span></span>
* <span data-ttu-id="96718-315">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-315">Added `container start` command</span></span>
* <span data-ttu-id="96718-316">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="96718-316">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="96718-317">EventGrid</span><span class="sxs-lookup"><span data-stu-id="96718-317">EventGrid</span></span>
* <span data-ttu-id="96718-318">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-318">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="96718-319">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-319">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="96718-320">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="96718-320">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="96718-321">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="96718-321">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="96718-322">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="96718-322">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="96718-323">HDInsight</span><span class="sxs-lookup"><span data-stu-id="96718-323">HDInsight</span></span>
* <span data-ttu-id="96718-324">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-324">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="96718-325">[BREAKING CHANGE] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="96718-325">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="96718-326">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-326">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="96718-327">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-327">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="96718-328">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-328">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="96718-329">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-329">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="96718-330">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-330">IoT</span></span>
* <span data-ttu-id="96718-331">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-331">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="96718-332">Kusto</span><span class="sxs-lookup"><span data-stu-id="96718-332">Kusto</span></span>
* <span data-ttu-id="96718-333">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="96718-333">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-334">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-334">Monitor</span></span>
* <span data-ttu-id="96718-335">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="96718-335">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="96718-336">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-336">Profile</span></span>
* <span data-ttu-id="96718-337">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="96718-337">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="96718-338">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-338">Network</span></span>
* <span data-ttu-id="96718-339">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="96718-339">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="96718-340">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="96718-340">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="96718-341">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-341">Resource</span></span>
* <span data-ttu-id="96718-342">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-342">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="96718-343">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-343">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="96718-344">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="96718-344">SQL Virtual Machine</span></span>
* <span data-ttu-id="96718-345">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="96718-345">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="96718-346">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-346">Storage</span></span>
* <span data-ttu-id="96718-347">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="96718-347">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="96718-348">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="96718-348">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="96718-349">VM</span><span class="sxs-lookup"><span data-stu-id="96718-349">VM</span></span>
* <span data-ttu-id="96718-350">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="96718-350">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="96718-351">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-351">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="96718-352">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="96718-352">January 15, 2019</span></span>

<span data-ttu-id="96718-353">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="96718-353">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="96718-354">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-354">ACR</span></span>
* <span data-ttu-id="96718-355">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-355">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="96718-356">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-356">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="96718-357">[VERALTET] Parameter `--resource-group` wurde in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="96718-357">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="96718-358">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-358">ACS</span></span>
* <span data-ttu-id="96718-359">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-359">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-360">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-360">Appservice</span></span>
* <span data-ttu-id="96718-361">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="96718-361">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="96718-362">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="96718-362">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="96718-363">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="96718-363">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="96718-364">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-364">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="96718-365">Botservice</span><span class="sxs-lookup"><span data-stu-id="96718-365">Botservice</span></span>
* <span data-ttu-id="96718-366">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-366">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="96718-367">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="96718-367">Configure</span></span>
* <span data-ttu-id="96718-368">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-368">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-369">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-369">CosmosDB</span></span>
* <span data-ttu-id="96718-370">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-370">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="96718-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="96718-371">HDInsight</span></span>
* <span data-ttu-id="96718-372">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-372">Added commands for managing applications</span></span>
* <span data-ttu-id="96718-373">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-373">Added commands for managing script actions</span></span>
* <span data-ttu-id="96718-374">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-374">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="96718-375">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-375">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="96718-376">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-376">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="96718-377">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-377">Network</span></span>
* <span data-ttu-id="96718-378">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-378">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="96718-379">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="96718-379">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="96718-380">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-380">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="96718-381">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="96718-381">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="96718-382">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-382">Role</span></span>
* <span data-ttu-id="96718-383">[VERALTET] Das `--password`-Argument wurde für `create-for-rbac` als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="96718-383">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="96718-384">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="96718-384">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="96718-385">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="96718-385">Security</span></span>
* <span data-ttu-id="96718-386">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-386">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="96718-387">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-387">Storage</span></span>
* <span data-ttu-id="96718-388">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="96718-388">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="96718-389">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="96718-389">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="96718-390">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-390">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="96718-391">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-391">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="96718-392">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-392">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="96718-393">VM</span><span class="sxs-lookup"><span data-stu-id="96718-393">VM</span></span>
* <span data-ttu-id="96718-394">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="96718-394">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="96718-395">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-395">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="96718-396">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-396">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="96718-397">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="96718-397">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="96718-398">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="96718-398">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="96718-399">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="96718-399">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="96718-400">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="96718-400">December 20, 2018</span></span>

<span data-ttu-id="96718-401">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="96718-401">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="96718-402">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-402">Appservice</span></span>
* <span data-ttu-id="96718-403">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-403">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="96718-404">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-404">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="96718-405">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-405">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="96718-406">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="96718-406">IoTCentral</span></span>
* <span data-ttu-id="96718-407">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="96718-407">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="96718-408">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-408">Role</span></span>
* <span data-ttu-id="96718-409">[BREAKING CHANGE] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="96718-409">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="96718-410">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-410">SQL</span></span>
* <span data-ttu-id="96718-411">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-411">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="96718-412">VM</span><span class="sxs-lookup"><span data-stu-id="96718-412">VM</span></span>
* <span data-ttu-id="96718-413">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-413">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="96718-414">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="96718-414">December 18, 2018</span></span>

<span data-ttu-id="96718-415">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="96718-415">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="96718-416">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-416">ACR</span></span>
* <span data-ttu-id="96718-417">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-417">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="96718-418">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="96718-418">Condensed the table layout for task list</span></span>
* <span data-ttu-id="96718-419">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-419">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="96718-420">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-420">ACS</span></span>
* <span data-ttu-id="96718-421">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-421">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="96718-422">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-422">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="96718-423">[VERALTET] `az acs`-Befehle als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="96718-423">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="96718-424">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="96718-424">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="96718-425">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-425">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="96718-426">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-426">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-427">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-427">Appservice</span></span>
* <span data-ttu-id="96718-428">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="96718-428">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="96718-429">Botservice</span><span class="sxs-lookup"><span data-stu-id="96718-429">Botservice</span></span>
* <span data-ttu-id="96718-430">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-430">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="96718-431">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="96718-431">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="96718-432">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="96718-432">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="96718-433">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="96718-433">Reduced Kudu network calls</span></span>
* <span data-ttu-id="96718-434">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="96718-434">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-435">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-435">Consumption</span></span>
* <span data-ttu-id="96718-436">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="96718-436">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-437">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-437">CosmosDB</span></span>
* <span data-ttu-id="96718-438">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-438">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="96718-439">Karten</span><span class="sxs-lookup"><span data-stu-id="96718-439">Maps</span></span>
* <span data-ttu-id="96718-440">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-440">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="96718-441">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-441">Network</span></span>
* <span data-ttu-id="96718-442">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-442">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="96718-443">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="96718-443">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="96718-444">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-444">Resource</span></span>
* <span data-ttu-id="96718-445">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-445">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="96718-446">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-446">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-447">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-447">Storage</span></span>
*  <span data-ttu-id="96718-448">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-448">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-449">VM</span><span class="sxs-lookup"><span data-stu-id="96718-449">VM</span></span>
* <span data-ttu-id="96718-450">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="96718-450">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="96718-451">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="96718-451">December 4, 2018</span></span>

<span data-ttu-id="96718-452">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="96718-452">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="96718-453">Core</span><span class="sxs-lookup"><span data-stu-id="96718-453">Core</span></span>
* <span data-ttu-id="96718-454">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-454">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="96718-455">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-455">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-456">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-456">Appservice</span></span>
* <span data-ttu-id="96718-457">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="96718-457">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="96718-458">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="96718-458">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="96718-459">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-459">Network</span></span>
* <span data-ttu-id="96718-460">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-460">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="96718-461">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-461">Role</span></span>
* <span data-ttu-id="96718-462">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-462">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="96718-463">VM</span><span class="sxs-lookup"><span data-stu-id="96718-463">VM</span></span>
* <span data-ttu-id="96718-464">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-464">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="96718-465">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="96718-465">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="96718-466">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="96718-466">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="96718-467">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="96718-467">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="96718-468">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="96718-468">November 20, 2018</span></span>

<span data-ttu-id="96718-469">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="96718-469">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="96718-470">Core</span><span class="sxs-lookup"><span data-stu-id="96718-470">Core</span></span>
* <span data-ttu-id="96718-471">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-471">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="96718-472">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-472">ACR</span></span>
* <span data-ttu-id="96718-473">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-473">Added context token to task step</span></span>
* <span data-ttu-id="96718-474">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-474">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="96718-475">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-475">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-476">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-476">Appservice</span></span>
* <span data-ttu-id="96718-477">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-477">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="96718-478">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="96718-478">Updated the default `node_version`.</span></span> <span data-ttu-id="96718-479">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="96718-479">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="96718-480">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-480">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="96718-481">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="96718-481">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="96718-482">IotCentral</span><span class="sxs-lookup"><span data-stu-id="96718-482">IotCentral</span></span>
* <span data-ttu-id="96718-483">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-483">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-484">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-484">KeyVault</span></span>
* <span data-ttu-id="96718-485">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-485">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="96718-486">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-486">Network</span></span>
* <span data-ttu-id="96718-487">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-487">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="96718-488">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-488">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="96718-489">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-489">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="96718-490">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-490">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-491">Rdbms</span><span class="sxs-lookup"><span data-stu-id="96718-491">Rdbms</span></span>
* <span data-ttu-id="96718-492">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-492">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="96718-493">RBAC</span><span class="sxs-lookup"><span data-stu-id="96718-493">Rbac</span></span>
* <span data-ttu-id="96718-494">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-494">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="96718-495">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-495">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="96718-496">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-496">Storage</span></span>
* <span data-ttu-id="96718-497">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-497">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="96718-498">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="96718-498">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="96718-499">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="96718-499">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="96718-500">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="96718-500">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="96718-501">VM</span><span class="sxs-lookup"><span data-stu-id="96718-501">VM</span></span>
* <span data-ttu-id="96718-502">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-502">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="96718-503">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="96718-503">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="96718-504">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="96718-504">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="96718-505">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-505">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="96718-506">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-506">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="96718-507">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-507">Added `snapshot wait` command</span></span>
* <span data-ttu-id="96718-508">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-508">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="96718-509">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="96718-509">November 6, 2018</span></span>

<span data-ttu-id="96718-510">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="96718-510">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="96718-511">Core</span><span class="sxs-lookup"><span data-stu-id="96718-511">Core</span></span>
* <span data-ttu-id="96718-512">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-512">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="96718-513">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-513">ACR</span></span>
* <span data-ttu-id="96718-514">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-514">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="96718-515">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="96718-515">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="96718-516">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-516">ACS</span></span>
* <span data-ttu-id="96718-517">[BREAKING CHANGE] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="96718-517">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="96718-518">Advisor</span><span class="sxs-lookup"><span data-stu-id="96718-518">Advisor</span></span>
* <span data-ttu-id="96718-519">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="96718-519">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="96718-520">AMS</span><span class="sxs-lookup"><span data-stu-id="96718-520">AMS</span></span>
* <span data-ttu-id="96718-521">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-521">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="96718-522">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-522">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="96718-523">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-523">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="96718-524">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="96718-524">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="96718-525">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-525">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="96718-526">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-526">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="96718-527">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-527">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="96718-528">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="96718-528">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="96718-529">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-529">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="96718-530">[BREAKING CHANGE] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-530">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="96718-531">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="96718-531">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="96718-532">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="96718-532">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="96718-533">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="96718-533">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="96718-534">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="96718-534">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="96718-535">[BREAKING CHANGE] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="96718-535">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="96718-536">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="96718-536">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="96718-537">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="96718-537">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-538">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-538">AppService</span></span>
* <span data-ttu-id="96718-539">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="96718-539">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="96718-540">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="96718-540">Configure</span></span>
* <span data-ttu-id="96718-541">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-541">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="96718-542">Container</span><span class="sxs-lookup"><span data-stu-id="96718-542">Container</span></span>
* <span data-ttu-id="96718-543">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="96718-543">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="96718-544">EventHub</span><span class="sxs-lookup"><span data-stu-id="96718-544">EventHub</span></span>
* <span data-ttu-id="96718-545">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-545">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-546">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-546">Interactive</span></span>
* <span data-ttu-id="96718-547">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-547">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-548">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-548">Monitor</span></span>
* <span data-ttu-id="96718-549">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-549">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="96718-550">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-550">Network</span></span>
* <span data-ttu-id="96718-551">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-551">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="96718-552">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="96718-552">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="96718-553">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="96718-553">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="96718-554">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-554">Profile</span></span>
* <span data-ttu-id="96718-555">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-555">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-556">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-556">RDBMS</span></span>
* <span data-ttu-id="96718-557">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-557">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="96718-558">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-558">Resource</span></span>
* <span data-ttu-id="96718-559">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-559">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="96718-560">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-560">Role</span></span>
* <span data-ttu-id="96718-561">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-561">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="96718-562">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="96718-562">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="96718-563">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-563">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="96718-564">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-564">Storage</span></span>
* <span data-ttu-id="96718-565">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="96718-565">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-566">VM</span><span class="sxs-lookup"><span data-stu-id="96718-566">VM</span></span>
* <span data-ttu-id="96718-567">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-567">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="96718-568">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="96718-568">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="96718-569">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-569">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="96718-570">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="96718-570">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="96718-571">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="96718-571">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="96718-572">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-572">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="96718-573">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="96718-573">October 23, 2018</span></span>

<span data-ttu-id="96718-574">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="96718-574">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="96718-575">Core</span><span class="sxs-lookup"><span data-stu-id="96718-575">Core</span></span>
* <span data-ttu-id="96718-576">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="96718-576">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="96718-577">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="96718-577">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="96718-578">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-578">ACR</span></span>
* <span data-ttu-id="96718-579">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="96718-579">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-580">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-580">CDN</span></span>
* <span data-ttu-id="96718-581">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="96718-581">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="96718-582">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="96718-582">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="96718-583">Container</span><span class="sxs-lookup"><span data-stu-id="96718-583">Container</span></span>
* <span data-ttu-id="96718-584">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-584">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="96718-585">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="96718-585">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="96718-586">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-586">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="96718-587">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="96718-587">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="96718-588">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="96718-588">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="96718-589">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="96718-589">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="96718-590">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-590">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-591">CosmosDB</span></span>
* <span data-ttu-id="96718-592">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-592">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-593">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-593">Interactive</span></span>
* <span data-ttu-id="96718-594">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="96718-594">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="96718-595">IoT Central</span><span class="sxs-lookup"><span data-stu-id="96718-595">IoT Central</span></span>
* <span data-ttu-id="96718-596">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-596">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="96718-597">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="96718-597">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-598">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-598">Monitor</span></span>
* <span data-ttu-id="96718-599">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="96718-599">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="96718-600">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-600">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="96718-601">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-601">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="96718-602">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-602">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="96718-603">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-603">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="96718-604">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="96718-604">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="96718-605">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="96718-605">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="96718-606">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-606">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="96718-607">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-607">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="96718-608">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-608">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="96718-609">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-609">Network</span></span>
* <span data-ttu-id="96718-610">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-610">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="96718-611">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-611">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="96718-612">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96718-612">ServiceBus</span></span>
* <span data-ttu-id="96718-613">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-613">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="96718-614">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-614">SQL</span></span>
* <span data-ttu-id="96718-615">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="96718-615">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="96718-616">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-616">Storage</span></span>
* <span data-ttu-id="96718-617">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-617">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="96718-618">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-618">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="96718-619">VM</span><span class="sxs-lookup"><span data-stu-id="96718-619">VM</span></span>
* <span data-ttu-id="96718-620">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="96718-620">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="96718-621">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-621">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="96718-622">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-622">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="96718-623">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="96718-623">October 16, 2018</span></span>

<span data-ttu-id="96718-624">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="96718-624">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="96718-625">VM</span><span class="sxs-lookup"><span data-stu-id="96718-625">VM</span></span>
* <span data-ttu-id="96718-626">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="96718-626">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="96718-627">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="96718-627">October 9, 2018</span></span>

<span data-ttu-id="96718-628">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="96718-628">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="96718-629">Core</span><span class="sxs-lookup"><span data-stu-id="96718-629">Core</span></span>
* <span data-ttu-id="96718-630">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="96718-630">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="96718-631">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-631">ACR</span></span>
* <span data-ttu-id="96718-632">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-632">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="96718-633">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-633">ACS</span></span>
* <span data-ttu-id="96718-634">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="96718-634">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="96718-635">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="96718-635">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="96718-636">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="96718-636">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="96718-637">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="96718-637">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="96718-638">Container</span><span class="sxs-lookup"><span data-stu-id="96718-638">Container</span></span>
* <span data-ttu-id="96718-639">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="96718-639">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="96718-640">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-640">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="96718-641">Event Hub</span><span class="sxs-lookup"><span data-stu-id="96718-641">Event Hub</span></span>
* <span data-ttu-id="96718-642">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-642">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="96718-643">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-643">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="96718-644">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="96718-644">Extensions</span></span>
* <span data-ttu-id="96718-645">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="96718-645">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="96718-646">HDInsight</span><span class="sxs-lookup"><span data-stu-id="96718-646">HDInsight</span></span>
* <span data-ttu-id="96718-647">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-647">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="96718-648">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-648">IoT</span></span>
* <span data-ttu-id="96718-649">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-649">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-650">KeyVault</span></span>
* <span data-ttu-id="96718-651">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="96718-651">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="96718-652">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-652">Network</span></span>
* <span data-ttu-id="96718-653">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="96718-653">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="96718-654">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="96718-654">See #6052</span></span>
* <span data-ttu-id="96718-655">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="96718-655">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="96718-656">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="96718-656">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="96718-657">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-657">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="96718-658">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-658">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="96718-659">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="96718-659">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="96718-660">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-660">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="96718-661">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-661">Role</span></span>
* <span data-ttu-id="96718-662">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-662">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="96718-663">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-663">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="96718-664">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="96718-664">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="96718-665">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="96718-665">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="96718-666">Service Bus</span><span class="sxs-lookup"><span data-stu-id="96718-666">Service Bus</span></span>
* <span data-ttu-id="96718-667">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-667">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="96718-668">VM</span><span class="sxs-lookup"><span data-stu-id="96718-668">VM</span></span>
* <span data-ttu-id="96718-669">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-669">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="96718-670">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="96718-670">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="96718-671">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-671">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="96718-672">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-672">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="96718-673">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="96718-673">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="96718-674">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="96718-674">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="96718-675">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="96718-675">September 21, 2018</span></span>

<span data-ttu-id="96718-676">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="96718-676">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="96718-677">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-677">ACR</span></span>
* <span data-ttu-id="96718-678">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-678">Added ACR Task commands</span></span>
* <span data-ttu-id="96718-679">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-679">Added quick run command</span></span>
* <span data-ttu-id="96718-680">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-680">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="96718-681">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-681">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="96718-682">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-682">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="96718-683">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-683">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="96718-684">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-684">ACS</span></span>
* <span data-ttu-id="96718-685">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="96718-685">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="96718-686">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-686">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-687">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-687">AppService</span></span>

* <span data-ttu-id="96718-688">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="96718-688">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="96718-689">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-689">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="96718-690">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-690">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="96718-691">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-691">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="96718-692">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-692">Batch</span></span>
* <span data-ttu-id="96718-693">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-693">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="96718-694">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-694">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="96718-695">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-695">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="96718-696">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="96718-696">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="96718-697">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-697">Batch AI</span></span> 
* <span data-ttu-id="96718-698">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-698">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="96718-699">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="96718-699">Cognitive Services</span></span>
* <span data-ttu-id="96718-700">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-700">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="96718-701">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-701">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="96718-702">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-702">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="96718-703">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-703">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="96718-704">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-704">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="96718-705">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="96718-705">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="96718-706">Container</span><span class="sxs-lookup"><span data-stu-id="96718-706">Container</span></span>
* <span data-ttu-id="96718-707">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-707">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="96718-708">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-708">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="96718-709">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-709">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="96718-710">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="96718-710">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="96718-711">Data Lake</span><span class="sxs-lookup"><span data-stu-id="96718-711">Datalake</span></span>
* <span data-ttu-id="96718-712">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-712">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="96718-713">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="96718-713">Interactive Shell</span></span>
* <span data-ttu-id="96718-714">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-714">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="96718-715">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="96718-715">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="96718-716">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-716">IoT</span></span>
* <span data-ttu-id="96718-717">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-717">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="96718-718">Key Vault</span><span class="sxs-lookup"><span data-stu-id="96718-718">Key Vault</span></span>
* <span data-ttu-id="96718-719">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-719">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="96718-720">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-720">Network</span></span>
* <span data-ttu-id="96718-721">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-721">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="96718-722">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-722">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="96718-723">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-723">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="96718-724">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-724">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="96718-725">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-725">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="96718-726">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-726">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="96718-727">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-727">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="96718-728">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="96718-728">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="96718-729">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-729">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="96718-730">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-730">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="96718-731">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-731">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="96718-732">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-732">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="96718-733">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-733">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="96718-734">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="96718-734">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="96718-735">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-735">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="96718-736">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="96718-736">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="96718-737">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-737">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="96718-738">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-738">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-739">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-739">RDBMS</span></span>
* <span data-ttu-id="96718-740">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-740">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="96718-741">Reservierung</span><span class="sxs-lookup"><span data-stu-id="96718-741">Reservation</span></span>
* <span data-ttu-id="96718-742">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-742">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="96718-743">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-743">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="96718-744">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="96718-744">Manage App</span></span>
* <span data-ttu-id="96718-745">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="96718-745">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="96718-746">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="96718-746">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="96718-747">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-747">Role</span></span>
* <span data-ttu-id="96718-748">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-748">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="96718-749">SignalR</span><span class="sxs-lookup"><span data-stu-id="96718-749">SignalR</span></span>
* <span data-ttu-id="96718-750">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-750">First release</span></span>

### <a name="storage"></a><span data-ttu-id="96718-751">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-751">Storage</span></span>
* <span data-ttu-id="96718-752">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-752">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="96718-753">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-753">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="96718-754">VM</span><span class="sxs-lookup"><span data-stu-id="96718-754">VM</span></span>
* <span data-ttu-id="96718-755">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="96718-755">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="96718-756">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-756">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="96718-757">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="96718-757">August 28, 2018</span></span>

<span data-ttu-id="96718-758">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="96718-758">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="96718-759">Core</span><span class="sxs-lookup"><span data-stu-id="96718-759">Core</span></span>

* <span data-ttu-id="96718-760">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-760">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="96718-761">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-761">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="96718-762">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-762">ACR</span></span>

* <span data-ttu-id="96718-763">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-763">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="96718-764">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="96718-764">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="96718-765">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-765">ACS</span></span>

* <span data-ttu-id="96718-766">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="96718-766">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="96718-767">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="96718-767">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-768">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-768">AppService</span></span>

* <span data-ttu-id="96718-769">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-769">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="96718-770">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-770">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="96718-771">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-771">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="96718-772">Backup</span><span class="sxs-lookup"><span data-stu-id="96718-772">Backup</span></span>

* <span data-ttu-id="96718-773">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-773">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="96718-774">Botdienst</span><span class="sxs-lookup"><span data-stu-id="96718-774">Bot Service</span></span>

* <span data-ttu-id="96718-775">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="96718-775">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="96718-776">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="96718-776">Cognitive Services</span></span>

* <span data-ttu-id="96718-777">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="96718-777">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="96718-778">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-778">IoT</span></span>

* <span data-ttu-id="96718-779">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="96718-779">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-780">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-780">Monitor</span></span>

* <span data-ttu-id="96718-781">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-781">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="96718-782">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-782">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="96718-783">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-783">Network</span></span>

* <span data-ttu-id="96718-784">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-784">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="96718-785">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-785">Resource</span></span>

* <span data-ttu-id="96718-786">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-786">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="96718-787">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-787">Storage</span></span>

* <span data-ttu-id="96718-788">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-788">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="96718-789">VM</span><span class="sxs-lookup"><span data-stu-id="96718-789">VM</span></span>

* <span data-ttu-id="96718-790">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="96718-790">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="96718-791">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="96718-791">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="96718-792">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="96718-792">Auguest 14, 2018</span></span>

<span data-ttu-id="96718-793">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="96718-793">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="96718-794">Core</span><span class="sxs-lookup"><span data-stu-id="96718-794">Core</span></span>

* <span data-ttu-id="96718-795">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-795">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="96718-796">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-796">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="96718-797">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="96718-797">Telemetry</span></span>

* <span data-ttu-id="96718-798">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="96718-798">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="96718-799">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-799">ACR</span></span>

* <span data-ttu-id="96718-800">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-800">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="96718-801">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="96718-801">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="96718-802">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-802">ACS</span></span>

* <span data-ttu-id="96718-803">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="96718-803">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="96718-804">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="96718-804">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="96718-805">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="96718-805">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="96718-806">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="96718-806">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="96718-807">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="96718-807">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="96718-808">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-808">AppService</span></span>

* <span data-ttu-id="96718-809">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="96718-809">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="96718-810">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="96718-810">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="96718-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-811">BatchAI</span></span>

* <span data-ttu-id="96718-812">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="96718-812">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="96718-813">Container</span><span class="sxs-lookup"><span data-stu-id="96718-813">Container</span></span>

* <span data-ttu-id="96718-814">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-814">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="96718-815">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-815">IoT</span></span>

* <span data-ttu-id="96718-816">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="96718-816">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="96718-817">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="96718-817">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="96718-818">Iot Central</span><span class="sxs-lookup"><span data-stu-id="96718-818">Iot Central</span></span>

* <span data-ttu-id="96718-819">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-819">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-820">KeyVault</span></span>


* <span data-ttu-id="96718-821">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-821">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="96718-822">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-822">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="96718-823">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-823">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="96718-824">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-824">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="96718-825">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-825">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="96718-826">Relay</span><span class="sxs-lookup"><span data-stu-id="96718-826">Relay</span></span>

* <span data-ttu-id="96718-827">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-827">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="96718-828">Sql</span><span class="sxs-lookup"><span data-stu-id="96718-828">Sql</span></span>

* <span data-ttu-id="96718-829">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-829">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="96718-830">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-830">Storage</span></span>

* <span data-ttu-id="96718-831">[BREAKING CHANGE] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="96718-831">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="96718-832">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="96718-832">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="96718-833">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-833">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="96718-834">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="96718-834">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="96718-835">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="96718-835">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="96718-836">VM</span><span class="sxs-lookup"><span data-stu-id="96718-836">VM</span></span>

* <span data-ttu-id="96718-837">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-837">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="96718-838">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="96718-838">July 31, 2018</span></span>

<span data-ttu-id="96718-839">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="96718-839">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="96718-840">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-840">ACR</span></span>

* <span data-ttu-id="96718-841">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-841">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="96718-842">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-842">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="96718-843">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-843">ACS</span></span>

* <span data-ttu-id="96718-844">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-844">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="96718-845">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-845">Batch</span></span>

* <span data-ttu-id="96718-846">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="96718-846">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="96718-847">Container</span><span class="sxs-lookup"><span data-stu-id="96718-847">Container</span></span>

* <span data-ttu-id="96718-848">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-848">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="96718-849">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-849">Network</span></span>

* <span data-ttu-id="96718-850">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-850">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="96718-851">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-851">Resource</span></span>

* <span data-ttu-id="96718-852">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="96718-852">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="96718-853">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="96718-853">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="96718-854">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-854">Role</span></span>

* <span data-ttu-id="96718-855">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-855">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="96718-856">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="96718-856">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="96718-857">Suchen,</span><span class="sxs-lookup"><span data-stu-id="96718-857">Search</span></span>

* <span data-ttu-id="96718-858">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-858">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="96718-859">Service Bus</span><span class="sxs-lookup"><span data-stu-id="96718-859">Service Bus</span></span>

* <span data-ttu-id="96718-860">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="96718-860">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="96718-861">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-861">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="96718-862">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="96718-862">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="96718-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="96718-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-864">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-864">Storage</span></span>

* <span data-ttu-id="96718-865">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-865">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="96718-866">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="96718-866">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="96718-867">VM</span><span class="sxs-lookup"><span data-stu-id="96718-867">VM</span></span>

* <span data-ttu-id="96718-868">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-868">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="96718-869">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-869">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="96718-870">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-870">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="96718-871">[BREAKING CHANGE] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="96718-871">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="96718-872">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="96718-872">July 18, 2018</span></span>

<span data-ttu-id="96718-873">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="96718-873">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="96718-874">Core</span><span class="sxs-lookup"><span data-stu-id="96718-874">Core</span></span>

* <span data-ttu-id="96718-875">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-875">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="96718-876">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-876">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="96718-877">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="96718-877">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="96718-878">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-878">ACR</span></span>

* <span data-ttu-id="96718-879">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="96718-879">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="96718-880">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-880">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="96718-881">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-881">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="96718-882">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-882">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="96718-883">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-883">ACS</span></span>

* <span data-ttu-id="96718-884">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="96718-884">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-885">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-885">AppService</span></span>

* <span data-ttu-id="96718-886">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-886">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="96718-887">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-887">Batch</span></span>

* <span data-ttu-id="96718-888">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="96718-888">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="96718-889">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="96718-889">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="96718-890">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-890">Batch AI</span></span>

* <span data-ttu-id="96718-891">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-891">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="96718-892">Container</span><span class="sxs-lookup"><span data-stu-id="96718-892">Container</span></span>

* <span data-ttu-id="96718-893">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-893">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="96718-894">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="96718-894">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="96718-895">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-895">Network</span></span>

* <span data-ttu-id="96718-896">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-896">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="96718-897">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-897">Added `network nic wait`</span></span>
* <span data-ttu-id="96718-898">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-898">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="96718-899">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="96718-899">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="96718-900">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-900">Resource</span></span>

* <span data-ttu-id="96718-901">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-901">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="96718-902">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-902">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="96718-903">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-903">Added `deployment wait` command</span></span>
* <span data-ttu-id="96718-904">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-904">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="96718-905">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-905">SQL</span></span>

* <span data-ttu-id="96718-906">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="96718-906">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="96718-907">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="96718-907">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="96718-908">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-908">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="96718-909">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-909">Storage</span></span>

* <span data-ttu-id="96718-910">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="96718-910">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="96718-911">VM</span><span class="sxs-lookup"><span data-stu-id="96718-911">VM</span></span>

* <span data-ttu-id="96718-912">[BREAKING CHANGE] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-912">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="96718-913">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-913">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="96718-914">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-914">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="96718-915">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="96718-915">July 3, 2018</span></span>

<span data-ttu-id="96718-916">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="96718-916">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="96718-917">AKS</span><span class="sxs-lookup"><span data-stu-id="96718-917">AKS</span></span>

* <span data-ttu-id="96718-918">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-918">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="96718-919">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="96718-919">July 3, 2018</span></span>

<span data-ttu-id="96718-920">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="96718-920">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="96718-921">Core</span><span class="sxs-lookup"><span data-stu-id="96718-921">Core</span></span>

* <span data-ttu-id="96718-922">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-922">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="96718-923">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-923">ACR</span></span>

* <span data-ttu-id="96718-924">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-924">Added polling build status</span></span>
* <span data-ttu-id="96718-925">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-925">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="96718-926">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-926">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="96718-927">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-927">ACS</span></span>

* <span data-ttu-id="96718-928">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="96718-928">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="96718-929">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="96718-929">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="96718-930">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="96718-930">Updated options for `aks browse` command.</span></span> <span data-ttu-id="96718-931">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-931">Added `--listen-port` support</span></span>
* <span data-ttu-id="96718-932">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="96718-932">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="96718-933">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="96718-933">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="96718-934">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-934">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-935">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-935">AppService</span></span>

* <span data-ttu-id="96718-936">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-936">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="96718-937">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-937">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="96718-938">Backup</span><span class="sxs-lookup"><span data-stu-id="96718-938">Backup</span></span>

* <span data-ttu-id="96718-939">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-939">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="96718-940">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-940">BatchAI</span></span>

* <span data-ttu-id="96718-941">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-941">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="96718-942">Cloud</span><span class="sxs-lookup"><span data-stu-id="96718-942">Cloud</span></span>

* <span data-ttu-id="96718-943">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-943">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="96718-944">Container</span><span class="sxs-lookup"><span data-stu-id="96718-944">Container</span></span>

* <span data-ttu-id="96718-945">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="96718-945">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="96718-946">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-946">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="96718-947">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-947">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="96718-948">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-948">Extension</span></span>

* <span data-ttu-id="96718-949">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="96718-949">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="96718-950">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-950">Network</span></span>

* <span data-ttu-id="96718-951">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="96718-951">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-952">Rdbms</span><span class="sxs-lookup"><span data-stu-id="96718-952">Rdbms</span></span>

* <span data-ttu-id="96718-953">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-953">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="96718-954">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-954">Resource</span></span>

* <span data-ttu-id="96718-955">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-955">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-956">VM</span><span class="sxs-lookup"><span data-stu-id="96718-956">VM</span></span>

* <span data-ttu-id="96718-957">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-957">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="96718-958">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-958">June 25, 2018</span></span>

<span data-ttu-id="96718-959">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="96718-959">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="96718-960">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="96718-960">CLI</span></span>

* <span data-ttu-id="96718-961">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="96718-961">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="96718-962">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-962">June 19, 2018</span></span>

<span data-ttu-id="96718-963">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="96718-963">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="96718-964">Core</span><span class="sxs-lookup"><span data-stu-id="96718-964">Core</span></span>

* <span data-ttu-id="96718-965">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-965">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="96718-966">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-966">ACR</span></span>

* <span data-ttu-id="96718-967">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-967">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="96718-968">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="96718-968">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="96718-969">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-969">ACS</span></span>

* <span data-ttu-id="96718-970">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="96718-970">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="96718-971">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-971">Added `--update` support</span></span>
* <span data-ttu-id="96718-972">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="96718-972">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="96718-973">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-973">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="96718-974">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-974">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="96718-975">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="96718-975">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="96718-976">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-976">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="96718-977">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-977">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-978">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-978">AppService</span></span>

* <span data-ttu-id="96718-979">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-979">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="96718-980">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-980">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="96718-981">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-981">Batch</span></span>

* <span data-ttu-id="96718-982">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-982">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="96718-983">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-983">Batch AI</span></span>

* <span data-ttu-id="96718-984">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-984">Added support for workspaces.</span></span> <span data-ttu-id="96718-985">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="96718-985">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="96718-986">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-986">Added support for experiments.</span></span> <span data-ttu-id="96718-987">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="96718-987">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="96718-988">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="96718-988">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="96718-989">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-989">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="96718-990">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="96718-990">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="96718-991">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-991">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="96718-992">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="96718-992">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="96718-993">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="96718-993">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="96718-994">[BREAKING CHANGE] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-994">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="96718-995">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="96718-995">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="96718-996">[BREAKING CHANGE] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-996">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="96718-997">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="96718-997">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="96718-998">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-998">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="96718-999">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="96718-999">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="96718-1000">[BREAKING CHANGE] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-1000">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="96718-1001">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="96718-1001">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="96718-1002">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1002">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="96718-1003">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1003">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="96718-1004">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1004">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="96718-1005">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1005">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="96718-1006">Karten</span><span class="sxs-lookup"><span data-stu-id="96718-1006">Maps</span></span>

* <span data-ttu-id="96718-1007">[BREAKING CHANGE] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="96718-1007">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="96718-1008">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1008">Network</span></span>

* <span data-ttu-id="96718-1009">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="96718-1009">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="96718-1010">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="96718-1010">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="96718-1011">#6502</span><span class="sxs-lookup"><span data-stu-id="96718-1011">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="96718-1012">Reservations</span><span class="sxs-lookup"><span data-stu-id="96718-1012">Reservations</span></span>

* <span data-ttu-id="96718-1013">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1013">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="96718-1014">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1014">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="96718-1015">[BREAKING CHANGE] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1015">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="96718-1016">[BREAKING CHANGE] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1016">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="96718-1017">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1017">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="96718-1018">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1018">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="96718-1019">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1019">Role</span></span>

* <span data-ttu-id="96718-1020">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1020">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1021">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1021">SQL</span></span>

* <span data-ttu-id="96718-1022">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="96718-1022">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1023">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1023">Storage</span></span>

* <span data-ttu-id="96718-1024">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1024">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1025">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1025">VM</span></span>

* <span data-ttu-id="96718-1026">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="96718-1026">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="96718-1027">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="96718-1027">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="96718-1028">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="96718-1028">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="96718-1029">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1029">June 13, 2018</span></span>

<span data-ttu-id="96718-1030">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="96718-1030">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="96718-1031">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1031">Core</span></span>

* <span data-ttu-id="96718-1032">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="96718-1032">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="96718-1033">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1033">June 13, 2018</span></span>

<span data-ttu-id="96718-1034">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="96718-1034">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="96718-1035">AKS</span><span class="sxs-lookup"><span data-stu-id="96718-1035">AKS</span></span>

* <span data-ttu-id="96718-1036">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1036">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="96718-1037">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1037">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="96718-1038">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1038">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="96718-1039">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1039">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="96718-1040">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1040">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1041">AppService</span></span>

* <span data-ttu-id="96718-1042">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1042">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="96718-1043">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1043">June 5, 2018</span></span>

<span data-ttu-id="96718-1044">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="96718-1044">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1045">Interactive</span></span>

* <span data-ttu-id="96718-1046">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1046">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="96718-1047">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1047">June 5, 2018</span></span>

<span data-ttu-id="96718-1048">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="96718-1048">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="96718-1049">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1049">Core</span></span>

* <span data-ttu-id="96718-1050">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1050">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="96718-1051">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="96718-1051">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1052">ACR</span></span>

* <span data-ttu-id="96718-1053">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1053">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="96718-1054">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1054">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="96718-1055">AKS</span><span class="sxs-lookup"><span data-stu-id="96718-1055">AKS</span></span>

* <span data-ttu-id="96718-1056">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="96718-1056">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1057">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1057">Batch</span></span>

* <span data-ttu-id="96718-1058">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="96718-1058">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="96718-1059">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-1059">IOT</span></span>

* <span data-ttu-id="96718-1060">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1060">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="96718-1061">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1061">Network</span></span>

* <span data-ttu-id="96718-1062">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="96718-1062">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="96718-1063">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="96718-1063">Policy Insights</span></span>

* <span data-ttu-id="96718-1064">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1064">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="96718-1065">ARM</span><span class="sxs-lookup"><span data-stu-id="96718-1065">ARM</span></span>

* <span data-ttu-id="96718-1066">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1066">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1067">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1067">SQL</span></span>

* <span data-ttu-id="96718-1068">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-1068">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="96718-1069">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-1069">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="96718-1070">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1070">Storage</span></span>

* <span data-ttu-id="96718-1071">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="96718-1071">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1072">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1072">VM</span></span>

* <span data-ttu-id="96718-1073">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="96718-1073">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="96718-1074">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1074">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="96718-1075">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1075">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="96718-1076">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1076">May 22, 2018</span></span>

<span data-ttu-id="96718-1077">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="96718-1077">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="96718-1078">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1078">Core</span></span>

* <span data-ttu-id="96718-1079">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1079">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1080">ACS</span></span>

* <span data-ttu-id="96718-1081">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1081">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="96718-1082">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1082">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1083">AppService</span></span>

* <span data-ttu-id="96718-1084">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="96718-1084">Improved generic update commands</span></span>
* <span data-ttu-id="96718-1085">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1085">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="96718-1086">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1086">Container</span></span>

* <span data-ttu-id="96718-1087">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1087">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="96718-1088">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1088">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1089">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1089">Extension</span></span>

* <span data-ttu-id="96718-1090">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="96718-1090">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1091">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1091">Interactive</span></span>

* <span data-ttu-id="96718-1092">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="96718-1092">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="96718-1093">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="96718-1093">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-1094">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-1094">KeyVault</span></span>

* <span data-ttu-id="96718-1095">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="96718-1095">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="96718-1096">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1096">Network</span></span>

* <span data-ttu-id="96718-1097">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="96718-1097">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="96718-1098">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="96718-1098">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1099">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1099">SQL</span></span>

* <span data-ttu-id="96718-1100">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="96718-1100">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="96718-1101">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1101">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="96718-1102">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1102">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="96718-1103">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="96718-1103">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="96718-1104">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="96718-1104">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="96718-1105">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="96718-1105">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="96718-1106">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="96718-1106">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="96718-1107">`edition`.</span><span class="sxs-lookup"><span data-stu-id="96718-1107">`edition`.</span></span> <span data-ttu-id="96718-1108">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="96718-1108">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="96718-1109">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="96718-1109">`elasticPoolName`.</span></span> <span data-ttu-id="96718-1110">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="96718-1110">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="96718-1111">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="96718-1111">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="96718-1112">`edition`.</span><span class="sxs-lookup"><span data-stu-id="96718-1112">`edition`.</span></span> <span data-ttu-id="96718-1113">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="96718-1113">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="96718-1114">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="96718-1114">`dtu`.</span></span> <span data-ttu-id="96718-1115">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="96718-1115">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="96718-1116">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="96718-1116">`databaseDtuMin`.</span></span> <span data-ttu-id="96718-1117">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="96718-1117">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="96718-1118">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="96718-1118">`databaseDtuMax`.</span></span> <span data-ttu-id="96718-1119">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="96718-1119">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="96718-1120">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1120">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="96718-1121">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1121">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1122">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1122">Storage</span></span>

* <span data-ttu-id="96718-1123">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1123">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="96718-1124">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1124">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1125">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1125">VM</span></span>

* <span data-ttu-id="96718-1126">[BREAKING CHANGE] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-1126">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="96718-1127">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="96718-1127">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="96718-1128">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1128">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="96718-1129">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1129">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="96718-1130">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1130">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="96718-1131">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1131">May 7, 2018</span></span>

<span data-ttu-id="96718-1132">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="96718-1132">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="96718-1133">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1133">Core</span></span>

* <span data-ttu-id="96718-1134">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="96718-1134">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="96718-1135">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1135">Added limited support for positional arguments</span></span>
* <span data-ttu-id="96718-1136">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-1136">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="96718-1137">#5591</span><span class="sxs-lookup"><span data-stu-id="96718-1137">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="96718-1138">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1138">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="96718-1139">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="96718-1139">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="96718-1140">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="96718-1140">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="96718-1141">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="96718-1141">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="96718-1142">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1142">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1143">ACR</span></span>

* <span data-ttu-id="96718-1144">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1144">Added ACR Build commands</span></span>
* <span data-ttu-id="96718-1145">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1145">Improved resource not found error messages</span></span>
* <span data-ttu-id="96718-1146">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="96718-1146">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="96718-1147">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="96718-1147">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="96718-1148">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="96718-1148">Improved repository commands error messages</span></span>
* <span data-ttu-id="96718-1149">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1149">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1150">ACS</span></span>

* <span data-ttu-id="96718-1151">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="96718-1151">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="96718-1152">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="96718-1152">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="96718-1153">AMS</span><span class="sxs-lookup"><span data-stu-id="96718-1153">AMS</span></span>

* <span data-ttu-id="96718-1154">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="96718-1154">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1155">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1155">Appservice</span></span>

* <span data-ttu-id="96718-1156">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="96718-1156">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="96718-1157">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1157">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="96718-1158">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1158">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="96718-1159">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1159">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="96718-1160">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-1160">Batch AI</span></span>

* <span data-ttu-id="96718-1161">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="96718-1161">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="96718-1162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="96718-1162">Cognitive Services</span></span>

* <span data-ttu-id="96718-1163">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="96718-1163">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-1164">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-1164">Consumption</span></span>

* <span data-ttu-id="96718-1165">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1165">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="96718-1166">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1166">Container</span></span>

* <span data-ttu-id="96718-1167">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="96718-1167">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="96718-1168">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="96718-1168">Cosmos DB</span></span>

* <span data-ttu-id="96718-1169">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="96718-1169">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="96718-1170">DMS</span><span class="sxs-lookup"><span data-stu-id="96718-1170">DMS</span></span>

* <span data-ttu-id="96718-1171">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96718-1171">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1172">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1172">Extension</span></span>

* <span data-ttu-id="96718-1173">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1173">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1174">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1174">Interactive</span></span>

* <span data-ttu-id="96718-1175">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="96718-1175">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="96718-1176">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="96718-1176">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="96718-1177">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1177">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="96718-1178">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1178">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="96718-1179">Labor</span><span class="sxs-lookup"><span data-stu-id="96718-1179">Lab</span></span>

* <span data-ttu-id="96718-1180">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1180">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="96718-1181">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1181">Network</span></span>

* <span data-ttu-id="96718-1182">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="96718-1182">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="96718-1183">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1183">Profile</span></span>

* <span data-ttu-id="96718-1184">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1184">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="96718-1185">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="96718-1185">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="96718-1186">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1186">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="96718-1187">Redis</span><span class="sxs-lookup"><span data-stu-id="96718-1187">Redis</span></span>

* <span data-ttu-id="96718-1188">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="96718-1188">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="96718-1189">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1189">Deprecated `redis list-all`.</span></span> <span data-ttu-id="96718-1190">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="96718-1190">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="96718-1191">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="96718-1191">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="96718-1192">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1192">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="96718-1193">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1193">Role</span></span>

* <span data-ttu-id="96718-1194">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1194">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1195">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1195">Storage</span></span>

* <span data-ttu-id="96718-1196">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="96718-1196">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="96718-1197">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="96718-1197">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="96718-1198">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="96718-1198">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="96718-1199">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="96718-1199">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="96718-1200">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="96718-1200">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1201">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1201">VM</span></span>

* <span data-ttu-id="96718-1202">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1202">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="96718-1203">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1203">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="96718-1204">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="96718-1204">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="96718-1205">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1205">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="96718-1206">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="96718-1206">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="96718-1207">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1207">Added write accelerator support</span></span>
* <span data-ttu-id="96718-1208">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1208">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="96718-1209">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="96718-1209">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="96718-1210">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="96718-1210">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="96718-1211">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1211">April 10, 2018</span></span>

<span data-ttu-id="96718-1212">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="96718-1212">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1213">ACR</span></span>

* <span data-ttu-id="96718-1214">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="96718-1214">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1215">ACS</span></span>

* <span data-ttu-id="96718-1216">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1216">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1217">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1217">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="96718-1219">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1219">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="96718-1220">Batch AI</span><span class="sxs-lookup"><span data-stu-id="96718-1220">BatchAI</span></span>

* <span data-ttu-id="96718-1221">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1221">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="96718-1222">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="96718-1222">Job level mounting</span></span>
  - <span data-ttu-id="96718-1223">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="96718-1223">Environment variables with secret values</span></span>
  - <span data-ttu-id="96718-1224">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="96718-1224">Performance counters settings</span></span>
  - <span data-ttu-id="96718-1225">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="96718-1225">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="96718-1226">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="96718-1226">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="96718-1227">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="96718-1227">Usage and limits reporting</span></span>
  - <span data-ttu-id="96718-1228">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="96718-1228">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="96718-1229">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="96718-1229">Support for custom images</span></span>
  - <span data-ttu-id="96718-1230">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1230">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="96718-1231">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="96718-1231">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="96718-1232">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="96718-1232">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="96718-1233">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="96718-1233">National clouds are supported</span></span>
* <span data-ttu-id="96718-1234">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1234">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="96718-1235">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="96718-1235">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="96718-1236">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1236">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="96718-1237">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="96718-1237">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="96718-1238">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="96718-1238">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="96718-1239">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="96718-1239">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="96718-1240">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="96718-1240">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="96718-1241">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1241">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="96718-1242">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="96718-1242">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="96718-1243">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1243">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="96718-1244">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="96718-1244">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="96718-1245">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="96718-1245">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="96718-1246">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="96718-1246">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="96718-1247">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="96718-1247">Billing</span></span>

* <span data-ttu-id="96718-1248">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1248">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-1249">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-1249">Consumption</span></span>

* <span data-ttu-id="96718-1250">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1250">Added `marketplace` commands</span></span>
* <span data-ttu-id="96718-1251">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1251">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="96718-1252">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1252">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="96718-1253">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1253">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="96718-1254">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1254">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="96718-1255">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1255">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="96718-1256">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1256">Container</span></span>

* <span data-ttu-id="96718-1257">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1257">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="96718-1258">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="96718-1258">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1259">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1259">Extension</span></span>

* <span data-ttu-id="96718-1260">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1260">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1261">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1261">Interactive</span></span>

* <span data-ttu-id="96718-1262">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="96718-1262">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="96718-1263">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1263">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="96718-1264">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1264">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="96718-1265">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1265">Network</span></span>

* <span data-ttu-id="96718-1266">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="96718-1266">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="96718-1267">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1267">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="96718-1268">#4910</span><span class="sxs-lookup"><span data-stu-id="96718-1268">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="96718-1269">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1269">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="96718-1270">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1270">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="96718-1271">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1271">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="96718-1272">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1272">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="96718-1273">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1273">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1274">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1274">Profile</span></span>

* <span data-ttu-id="96718-1275">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1275">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="96718-1276">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1276">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-1277">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-1277">RDBMS</span></span>

* <span data-ttu-id="96718-1278">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1278">Added `georestore` command</span></span>
* <span data-ttu-id="96718-1279">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1279">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1280">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1280">Resource</span></span>

* <span data-ttu-id="96718-1281">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1281">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="96718-1282">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1282">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1283">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1283">SQL</span></span>

* <span data-ttu-id="96718-1284">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1284">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1285">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1285">Storage</span></span>

* <span data-ttu-id="96718-1286">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1286">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1287">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1287">VM</span></span>

* <span data-ttu-id="96718-1288">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1288">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="96718-1289">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="96718-1289">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="96718-1291">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1291">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="96718-1292">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="96718-1292">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="96718-1293">#5718</span><span class="sxs-lookup"><span data-stu-id="96718-1293">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="96718-1294">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="96718-1294">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="96718-1295">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1295">March 27, 2018</span></span>

<span data-ttu-id="96718-1296">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="96718-1296">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="96718-1297">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1297">Core</span></span>

* <span data-ttu-id="96718-1298">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="96718-1298">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1299">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1299">ACS</span></span>

* <span data-ttu-id="96718-1300">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="96718-1300">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1301">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1301">Appservice</span></span>

* <span data-ttu-id="96718-1302">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1302">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="96718-1303">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1303">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="96718-1304">Backup</span><span class="sxs-lookup"><span data-stu-id="96718-1304">Backup</span></span>

* <span data-ttu-id="96718-1305">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1305">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="96718-1306">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="96718-1306">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="96718-1307">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="96718-1307">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="96718-1308">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="96718-1308">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="96718-1309">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1309">Container</span></span>

* <span data-ttu-id="96718-1310">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1310">Added `container exec` command.</span></span> <span data-ttu-id="96718-1311">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="96718-1311">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="96718-1312">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="96718-1312">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1313">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1313">Extension</span></span>

* <span data-ttu-id="96718-1314">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="96718-1314">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="96718-1315">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-1315">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="96718-1316">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-1316">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1317">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1317">Interactive</span></span>

* <span data-ttu-id="96718-1318">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="96718-1318">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="96718-1319">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1319">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="96718-1320">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="96718-1320">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="96718-1321">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="96718-1321">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="96718-1322">Labor</span><span class="sxs-lookup"><span data-stu-id="96718-1322">Lab</span></span>

* <span data-ttu-id="96718-1323">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1323">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1324">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1324">Monitor</span></span>

* <span data-ttu-id="96718-1325">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="96718-1325">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="96718-1326">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="96718-1326">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="96718-1327">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="96718-1327">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="96718-1328">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1328">Network</span></span>

* <span data-ttu-id="96718-1329">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1329">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1330">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1330">Profile</span></span>

* <span data-ttu-id="96718-1331">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1331">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-1332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-1332">RDBMS</span></span>

* <span data-ttu-id="96718-1333">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1333">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1334">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1334">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="96718-1336">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1336">Role</span></span>

* <span data-ttu-id="96718-1337">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1337">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="96718-1338">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="96718-1338">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="96718-1339">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1339">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="96718-1340">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1340">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="96718-1341">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1341">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1342">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1342">Storage</span></span>

* <span data-ttu-id="96718-1343">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1343">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="96718-1344">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="96718-1344">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1345">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1345">VM</span></span>

* <span data-ttu-id="96718-1346">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1346">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="96718-1347">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1347">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="96718-1348">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="96718-1348">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="96718-1349">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="96718-1349">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="96718-1350">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1350">March 13, 2018</span></span>

<span data-ttu-id="96718-1351">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="96718-1351">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1352">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1352">ACR</span></span>

* <span data-ttu-id="96718-1353">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1353">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="96718-1354">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1354">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="96718-1355">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1355">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1356">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1356">ACS</span></span>

* <span data-ttu-id="96718-1357">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1357">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="96718-1358">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1358">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="96718-1359">Advisor</span><span class="sxs-lookup"><span data-stu-id="96718-1359">Advisor</span></span>

* <span data-ttu-id="96718-1360">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1360">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="96718-1361">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1361">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="96718-1362">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1362">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="96718-1363">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1363">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="96718-1364">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1364">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1365">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1365">Appservice</span></span>

* <span data-ttu-id="96718-1366">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1366">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="96718-1367">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1367">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="96718-1368">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="96718-1368">Eventhubs</span></span>

* <span data-ttu-id="96718-1369">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1369">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1370">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1370">Extension</span></span>

* <span data-ttu-id="96718-1371">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="96718-1371">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1372">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1372">Interactive</span></span>

* <span data-ttu-id="96718-1373">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="96718-1373">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="96718-1374">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="96718-1374">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="96718-1375">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="96718-1375">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="96718-1376">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1376">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1377">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1377">Monitor</span></span>

* <span data-ttu-id="96718-1378">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1378">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="96718-1379">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1379">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="96718-1380">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1380">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="96718-1381">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1381">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="96718-1382">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1382">Network</span></span>

* <span data-ttu-id="96718-1383">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1383">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="96718-1384">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="96718-1384">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="96718-1385">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1385">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="96718-1386">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1386">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1387">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1387">Profile</span></span>

* <span data-ttu-id="96718-1388">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1388">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="96718-1389">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1389">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-1390">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-1390">RDBMS</span></span>

* <span data-ttu-id="96718-1391">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-1391">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="96718-1392">Service Bus</span><span class="sxs-lookup"><span data-stu-id="96718-1392">Service Bus</span></span>

* <span data-ttu-id="96718-1393">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1393">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1394">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1394">Storage</span></span>

* <span data-ttu-id="96718-1395">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="96718-1395">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="96718-1396">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="96718-1396">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1397">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1397">VM</span></span>

* <span data-ttu-id="96718-1398">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="96718-1398">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="96718-1399">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="96718-1399">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="96718-1400">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1400">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="96718-1401">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1401">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="96718-1402">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1402">February 27, 2018</span></span>

<span data-ttu-id="96718-1403">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="96718-1403">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="96718-1404">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1404">Core</span></span>

* <span data-ttu-id="96718-1405">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="96718-1405">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="96718-1406">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1406">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="96718-1407">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1407">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1408">ACS</span></span>

* <span data-ttu-id="96718-1409">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-1409">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="96718-1410">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="96718-1410">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="96718-1411">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1411">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="96718-1412">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1412">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1413">Appservice</span></span>

* <span data-ttu-id="96718-1414">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="96718-1414">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="96718-1415">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="96718-1415">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="96718-1416">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="96718-1416">Cognitive Services</span></span>

* <span data-ttu-id="96718-1417">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1417">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-1418">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-1418">Consumption</span></span>

* <span data-ttu-id="96718-1419">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1419">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="96718-1420">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1420">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="96718-1421">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1421">Container</span></span>

* <span data-ttu-id="96718-1422">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="96718-1422">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="96718-1423">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1423">Network</span></span>

* <span data-ttu-id="96718-1424">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="96718-1424">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1425">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1425">Resource</span></span>

* <span data-ttu-id="96718-1426">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="96718-1426">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="96718-1427">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1427">Role</span></span>

* <span data-ttu-id="96718-1428">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1428">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1429">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1429">SQL</span></span>

* <span data-ttu-id="96718-1430">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="96718-1430">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1431">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1431">Storage</span></span>

* <span data-ttu-id="96718-1432">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-1432">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1433">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1433">VM</span></span>

* <span data-ttu-id="96718-1434">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1434">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="96718-1435">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1435">February 13, 2018</span></span>

<span data-ttu-id="96718-1436">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="96718-1436">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="96718-1437">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1437">Core</span></span>

* <span data-ttu-id="96718-1438">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1438">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1439">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1439">ACS</span></span>

* <span data-ttu-id="96718-1440">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1440">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="96718-1441">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1441">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="96718-1442">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1442">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="96718-1443">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1443">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="96718-1444">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1444">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="96718-1445">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1445">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="96718-1446">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="96718-1446">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="96718-1447">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="96718-1447">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1448">Appservice</span></span>

* <span data-ttu-id="96718-1449">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="96718-1449">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="96718-1450">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1450">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-1451">CDN</span></span>

* <span data-ttu-id="96718-1452">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1452">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="96718-1453">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1453">Container</span></span>

* <span data-ttu-id="96718-1454">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1454">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="96718-1455">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1455">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-1456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-1456">CosmosDB</span></span>

* <span data-ttu-id="96718-1457">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1457">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1458">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1458">Extension</span></span>

* <span data-ttu-id="96718-1459">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1459">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="96718-1460">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1460">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="96718-1461">Feedback</span><span class="sxs-lookup"><span data-stu-id="96718-1461">Feedback</span></span>

* <span data-ttu-id="96718-1462">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1462">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1463">Interactive</span></span>

* <span data-ttu-id="96718-1464">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="96718-1464">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="96718-1465">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1465">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="96718-1466">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-1466">IoT</span></span>

* <span data-ttu-id="96718-1467">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="96718-1467">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="96718-1468">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="96718-1468">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="96718-1469">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1469">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="96718-1470">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1470">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1471">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1471">Monitor</span></span>

* <span data-ttu-id="96718-1472">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1472">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="96718-1473">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1473">Network</span></span>

* <span data-ttu-id="96718-1474">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="96718-1474">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="96718-1475">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1475">Profile</span></span>

* <span data-ttu-id="96718-1476">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="96718-1476">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1477">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1477">Resource</span></span>

* <span data-ttu-id="96718-1478">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1478">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="96718-1479">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1479">Role</span></span>

* <span data-ttu-id="96718-1480">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1480">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1481">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1481">SQL</span></span>

* <span data-ttu-id="96718-1482">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1482">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="96718-1483">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1483">Added `sql db rename`</span></span>
* <span data-ttu-id="96718-1484">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1484">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1485">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1485">Storage</span></span>

* <span data-ttu-id="96718-1486">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1486">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1487">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1487">VM</span></span>

* <span data-ttu-id="96718-1488">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1488">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="96718-1489">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1489">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="96718-1490">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="96718-1490">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="96718-1491">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1491">January 31, 2018</span></span>

<span data-ttu-id="96718-1492">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="96718-1492">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="96718-1493">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1493">Core</span></span>

* <span data-ttu-id="96718-1494">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1494">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="96718-1495">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1495">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="96718-1496">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="96718-1496">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="96718-1497">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="96718-1497">Use `--verbose` to see</span></span>
* <span data-ttu-id="96718-1498">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1498">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1499">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1499">ACS</span></span>

* <span data-ttu-id="96718-1500">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="96718-1500">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="96718-1501">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1501">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1502">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1502">Appservice</span></span>

* <span data-ttu-id="96718-1503">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="96718-1503">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="96718-1504">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1504">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-1505">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-1505">CDN</span></span>

* <span data-ttu-id="96718-1506">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1506">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-1507">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-1507">CosmosDB</span></span>

* <span data-ttu-id="96718-1508">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1508">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1509">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1509">Interactive</span></span>

* <span data-ttu-id="96718-1510">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1510">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="96718-1511">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1511">Network</span></span>

* <span data-ttu-id="96718-1512">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1512">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="96718-1513">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="96718-1513">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="96718-1514">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1514">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="96718-1515">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1515">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="96718-1516">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1516">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="96718-1517">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="96718-1517">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="96718-1518">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1518">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="96718-1519">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1519">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="96718-1520">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1520">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="96718-1521">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="96718-1521">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1522">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1522">Profile</span></span>

* <span data-ttu-id="96718-1523">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1523">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1524">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1524">Resource</span></span>

* <span data-ttu-id="96718-1525">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="96718-1525">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1526">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1526">Storage</span></span>

* <span data-ttu-id="96718-1527">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1527">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="96718-1528">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1528">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="96718-1529">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="96718-1529">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="96718-1530">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1530">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="96718-1531">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="96718-1531">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1532">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1532">VM</span></span>

* <span data-ttu-id="96718-1533">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1533">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="96718-1534">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="96718-1534">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="96718-1535">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1535">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="96718-1536">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1536">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="96718-1537">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="96718-1537">January 17, 2018</span></span>

<span data-ttu-id="96718-1538">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="96718-1538">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1539">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1539">ACR</span></span>

* <span data-ttu-id="96718-1540">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1540">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="96718-1541">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="96718-1541">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1542">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1542">ACS</span></span>

* <span data-ttu-id="96718-1543">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1543">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="96718-1544">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1544">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1545">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1545">Appservice</span></span>

* <span data-ttu-id="96718-1546">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="96718-1546">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="96718-1547">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1547">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="96718-1548">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1548">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="96718-1549">Backup</span><span class="sxs-lookup"><span data-stu-id="96718-1549">Backup</span></span>

* <span data-ttu-id="96718-1550">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="96718-1550">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="96718-1551">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1551">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="96718-1552">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="96718-1552">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="96718-1553">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="96718-1553">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="96718-1554">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="96718-1554">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1555">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1555">Batch</span></span>

* <span data-ttu-id="96718-1556">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="96718-1556">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="96718-1557">Cloud</span><span class="sxs-lookup"><span data-stu-id="96718-1557">Cloud</span></span>

* <span data-ttu-id="96718-1558">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="96718-1558">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-1559">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-1559">Consumption</span></span>

* <span data-ttu-id="96718-1560">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="96718-1560">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="96718-1561">Event Grid</span><span class="sxs-lookup"><span data-stu-id="96718-1561">Event Grid</span></span>

* <span data-ttu-id="96718-1562">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="96718-1562">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="96718-1563">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="96718-1563">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="96718-1564">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-1564">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="96718-1565">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="96718-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="96718-1566">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1566">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="96718-1567">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1567">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="96718-1568">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1568">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="96718-1569">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1569">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-1570">Interactive</span><span class="sxs-lookup"><span data-stu-id="96718-1570">Interactive</span></span>

* <span data-ttu-id="96718-1571">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-1571">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="96718-1572">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1572">Fixed errors on startup</span></span>
* <span data-ttu-id="96718-1573">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="96718-1573">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="96718-1574">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-1574">IoT</span></span>

* <span data-ttu-id="96718-1575">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1575">Added support for device provisioning service</span></span>
* <span data-ttu-id="96718-1576">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1576">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="96718-1577">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="96718-1577">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1578">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1578">Monitor</span></span>

* <span data-ttu-id="96718-1579">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1579">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="96718-1580">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96718-1580">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="96718-1581">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1581">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="96718-1582">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1582">Network</span></span>

* <span data-ttu-id="96718-1583">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="96718-1583">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="96718-1584">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1584">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1585">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1585">Profile</span></span>

* <span data-ttu-id="96718-1586">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1586">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="96718-1587">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1587">Role</span></span>

* <span data-ttu-id="96718-1588">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="96718-1588">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="96718-1589">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="96718-1589">Service Fabric</span></span>

* <span data-ttu-id="96718-1590">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1590">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="96718-1591">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1591">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1592">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1592">VM</span></span>

* <span data-ttu-id="96718-1593">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="96718-1593">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="96718-1594">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1594">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="96718-1595">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="96718-1595">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="96718-1596">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1596">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="96718-1597">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1597">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="96718-1598">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1598">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="96718-1599">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1599">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="96718-1600">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1600">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="96718-1601">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1601">December 19, 2017</span></span>

<span data-ttu-id="96718-1602">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="96718-1602">Version 2.0.23</span></span>

* <span data-ttu-id="96718-1603">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1603">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="96718-1604">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1604">Container</span></span>

* <span data-ttu-id="96718-1605">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1605">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="96718-1606">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1606">Network</span></span>

* <span data-ttu-id="96718-1607">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1607">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="96718-1608">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1608">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1609">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1609">Storage</span></span>

* <span data-ttu-id="96718-1610">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1610">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1611">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1611">VM</span></span>

* <span data-ttu-id="96718-1612">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1612">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="96718-1613">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1613">December 5, 2017</span></span>

<span data-ttu-id="96718-1614">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="96718-1614">Version 2.0.22</span></span>

* <span data-ttu-id="96718-1615">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-1615">Removed `az component` commands.</span></span> <span data-ttu-id="96718-1616">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="96718-1616">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="96718-1617">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1617">Core</span></span>
* <span data-ttu-id="96718-1618">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="96718-1618">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="96718-1619">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1619">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1620">ACS</span></span>

* <span data-ttu-id="96718-1621">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1621">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="96718-1622">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="96718-1622">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="96718-1623">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="96718-1623">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="96718-1624">Advisor</span><span class="sxs-lookup"><span data-stu-id="96718-1624">Advisor</span></span>

* <span data-ttu-id="96718-1625">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1625">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1626">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1626">Appservice</span></span>

* <span data-ttu-id="96718-1627">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="96718-1627">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="96718-1628">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="96718-1628">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="96718-1629">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1629">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="96718-1630">Nutzung</span><span class="sxs-lookup"><span data-stu-id="96718-1630">Consumption</span></span>

* <span data-ttu-id="96718-1631">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1631">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="96718-1632">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1632">Container</span></span>

* <span data-ttu-id="96718-1633">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="96718-1633">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1634">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1634">Monitor</span></span>

* <span data-ttu-id="96718-1635">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1635">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1636">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1636">Resource</span></span>

* <span data-ttu-id="96718-1637">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1637">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="96718-1638">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-1638">Role</span></span>

* <span data-ttu-id="96718-1639">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1639">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="96718-1640">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1640">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="96718-1641">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="96718-1641">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1642">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1642">SQL</span></span>

* <span data-ttu-id="96718-1643">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1643">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="96718-1644">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1644">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1645">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1645">VM</span></span>

* <span data-ttu-id="96718-1646">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1646">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="96718-1647">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1647">November 14, 2017</span></span>

<span data-ttu-id="96718-1648">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="96718-1648">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1649">ACR</span></span>

* <span data-ttu-id="96718-1650">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1650">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="96718-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1651">ACS</span></span>

* <span data-ttu-id="96718-1652">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1652">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="96718-1653">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="96718-1653">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="96718-1654">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="96718-1654">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="96718-1655">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1655">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="96718-1656">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1656">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1657">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1657">Appservice</span></span>

* <span data-ttu-id="96718-1658">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1658">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="96718-1659">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1659">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="96718-1660">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1660">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="96718-1661">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-1661">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="96718-1662">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1662">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="96718-1663">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="96718-1663">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1664">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1664">Batch</span></span>

* <span data-ttu-id="96718-1665">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="96718-1665">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="96718-1666">BatchAI</span><span class="sxs-lookup"><span data-stu-id="96718-1666">Batchai</span></span>

* <span data-ttu-id="96718-1667">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1667">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="96718-1668">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1668">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="96718-1669">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1669">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="96718-1670">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1670">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="96718-1671">Cloud</span><span class="sxs-lookup"><span data-stu-id="96718-1671">Cloud</span></span>

* <span data-ttu-id="96718-1672">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="96718-1672">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="96718-1673">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1673">Container</span></span>

* <span data-ttu-id="96718-1674">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1674">Added support to open multiple ports</span></span>
* <span data-ttu-id="96718-1675">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1675">Added container group restart policy</span></span>
* <span data-ttu-id="96718-1676">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1676">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="96718-1677">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1677">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="96718-1678">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="96718-1678">Data Lake Analytics</span></span>

* <span data-ttu-id="96718-1679">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="96718-1679">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="96718-1680">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="96718-1680">Data Lake Store</span></span>

* <span data-ttu-id="96718-1681">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="96718-1681">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1682">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1682">Extension</span></span>

* <span data-ttu-id="96718-1683">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1683">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="96718-1684">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="96718-1684">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="96718-1685">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-1685">IoT</span></span>

* <span data-ttu-id="96718-1686">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1686">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1687">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1687">Monitor</span></span>

* <span data-ttu-id="96718-1688">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1688">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="96718-1689">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1689">Network</span></span>

* <span data-ttu-id="96718-1690">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1690">Added support for CAA DNS records</span></span>
* <span data-ttu-id="96718-1691">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="96718-1691">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="96718-1692">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="96718-1692">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="96718-1693">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1693">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="96718-1694">Reservations</span><span class="sxs-lookup"><span data-stu-id="96718-1694">Reservations</span></span>

* <span data-ttu-id="96718-1695">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="96718-1695">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1696">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1696">Resource</span></span>

* <span data-ttu-id="96718-1697">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1697">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1698">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1698">SQL</span></span>

* <span data-ttu-id="96718-1699">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1699">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1700">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1700">Storage</span></span>

* <span data-ttu-id="96718-1701">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="96718-1701">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="96718-1702">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="96718-1702">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="96718-1703">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="96718-1703">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="96718-1704">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1704">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="96718-1705">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1705">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="96718-1706">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1706">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="96718-1707">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1707">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1708">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1708">VM</span></span>

* <span data-ttu-id="96718-1709">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="96718-1709">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="96718-1710">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1710">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="96718-1711">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="96718-1711">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="96718-1712">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1712">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="96718-1713">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1713">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="96718-1714">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1714">October 24, 2017</span></span>

<span data-ttu-id="96718-1715">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="96718-1715">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="96718-1716">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1716">Core</span></span>

* <span data-ttu-id="96718-1717">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="96718-1717">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1718">ACR</span></span>

* <span data-ttu-id="96718-1719">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="96718-1719">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="96718-1720">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="96718-1720">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="96718-1721">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="96718-1721">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1722">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1722">ACS</span></span>

* <span data-ttu-id="96718-1723">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1723">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="96718-1724">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1724">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1725">Appservice</span></span>

* <span data-ttu-id="96718-1726">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="96718-1726">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="96718-1727">Komponente</span><span class="sxs-lookup"><span data-stu-id="96718-1727">Component</span></span>

* <span data-ttu-id="96718-1728">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1728">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-1729">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-1729">Monitor</span></span>

* <span data-ttu-id="96718-1730">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1730">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1731">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1731">Resource</span></span>

* <span data-ttu-id="96718-1732">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1732">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="96718-1733">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="96718-1733">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1734">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1734">VM</span></span>

* <span data-ttu-id="96718-1735">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1735">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="96718-1736">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1736">October 9, 2017</span></span>

<span data-ttu-id="96718-1737">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="96718-1737">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="96718-1738">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1738">Core</span></span>

* <span data-ttu-id="96718-1739">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1739">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1740">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1740">Appservice</span></span>

* <span data-ttu-id="96718-1741">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-1741">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1742">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1742">Batch</span></span>

* <span data-ttu-id="96718-1743">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="96718-1743">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="96718-1744">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="96718-1744">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="96718-1745">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1745">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="96718-1746">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1746">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="96718-1747">BatchAI</span><span class="sxs-lookup"><span data-stu-id="96718-1747">Batchai</span></span>

* <span data-ttu-id="96718-1748">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-1748">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-1749">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-1749">Keyvault</span></span>

* <span data-ttu-id="96718-1750">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="96718-1750">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="96718-1751">(#4448)</span><span class="sxs-lookup"><span data-stu-id="96718-1751">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="96718-1752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1752">Network</span></span>

* <span data-ttu-id="96718-1753">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="96718-1753">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="96718-1754">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="96718-1754">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1755">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1755">Resource</span></span>

* <span data-ttu-id="96718-1756">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1756">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="96718-1757">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-1757">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="96718-1758">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-1758">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="96718-1759">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-1759">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1760">Sql</span><span class="sxs-lookup"><span data-stu-id="96718-1760">Sql</span></span>

* <span data-ttu-id="96718-1761">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1761">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="96718-1762">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-1762">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="96718-1763">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="96718-1763">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1764">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1764">Storage</span></span>

* <span data-ttu-id="96718-1765">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1765">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1766">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1766">Vm</span></span>

* <span data-ttu-id="96718-1767">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="96718-1767">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="96718-1768">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1768">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="96718-1769">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1769">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="96718-1770">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1770">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="96718-1771">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1771">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="96718-1772">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1772">September 22, 2017</span></span>

<span data-ttu-id="96718-1773">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="96718-1773">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1774">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1774">Resource</span></span>

* <span data-ttu-id="96718-1775">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1775">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="96718-1776">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1776">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="96718-1777">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1777">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="96718-1778">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="96718-1778">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="96718-1779">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1779">Network</span></span>

* <span data-ttu-id="96718-1780">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1780">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="96718-1781">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1781">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="96718-1782">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1782">Added `asg` application security group commands</span></span>
* <span data-ttu-id="96718-1783">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1783">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="96718-1784">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1784">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="96718-1785">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1785">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="96718-1786">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1786">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1787">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1787">Storage</span></span>

* <span data-ttu-id="96718-1788">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="96718-1788">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="96718-1789">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="96718-1789">Eventgrid</span></span>

* <span data-ttu-id="96718-1790">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1790">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1791">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1791">SQL</span></span>

* <span data-ttu-id="96718-1792">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="96718-1792">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="96718-1793">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96718-1793">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="96718-1794">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1794">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-1795">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-1795">Keyvault</span></span>

* <span data-ttu-id="96718-1796">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1796">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1797">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1797">VM</span></span>

* <span data-ttu-id="96718-1798">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1798">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="96718-1799">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="96718-1799">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="96718-1800">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1800">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="96718-1801">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1801">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="96718-1802">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1802">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="96718-1803">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1803">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1804">ACS</span></span>

* <span data-ttu-id="96718-1805">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1805">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1806">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1806">Appservice</span></span>

* <span data-ttu-id="96718-1807">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="96718-1807">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="96718-1808">Backup</span><span class="sxs-lookup"><span data-stu-id="96718-1808">Backup</span></span>

* <span data-ttu-id="96718-1809">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="96718-1809">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="96718-1810">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1810">September 11, 2017</span></span>

<span data-ttu-id="96718-1811">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="96718-1811">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="96718-1812">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1812">Core</span></span>

* <span data-ttu-id="96718-1813">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="96718-1813">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="96718-1814">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="96718-1814">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1815">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1815">Acs</span></span>

* <span data-ttu-id="96718-1816">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1816">Added `acs list-locations` command</span></span>
* <span data-ttu-id="96718-1817">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="96718-1817">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1818">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1818">Appservice</span></span>

* <span data-ttu-id="96718-1819">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="96718-1819">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-1820">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-1820">CDN</span></span>

* <span data-ttu-id="96718-1821">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="96718-1821">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="96718-1822">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="96718-1822">Extension</span></span>

* <span data-ttu-id="96718-1823">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1823">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-1824">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-1824">Keyvault</span></span>

* <span data-ttu-id="96718-1825">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="96718-1825">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="96718-1826">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1826">Network</span></span>

* <span data-ttu-id="96718-1827">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1827">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="96718-1828">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="96718-1828">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="96718-1829">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1829">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="96718-1830">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1830">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="96718-1831">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1831">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="96718-1832">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-1832">Resource</span></span>

* <span data-ttu-id="96718-1833">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="96718-1833">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="96718-1834">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="96718-1834">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="96718-1835">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="96718-1835">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="96718-1836">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="96718-1836">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="96718-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-1837">SQL</span></span>

* <span data-ttu-id="96718-1838">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1838">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1839">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1839">VM</span></span>

* <span data-ttu-id="96718-1840">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="96718-1840">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="96718-1841">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="96718-1841">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="96718-1842">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1842">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="96718-1843">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="96718-1843">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="96718-1844">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="96718-1844">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="96718-1845">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1845">August 31, 2017</span></span>

<span data-ttu-id="96718-1846">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="96718-1846">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-1847">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-1847">Keyvault</span></span>

* <span data-ttu-id="96718-1848">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="96718-1848">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="96718-1849">Sf</span><span class="sxs-lookup"><span data-stu-id="96718-1849">Sf</span></span>

* <span data-ttu-id="96718-1850">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="96718-1850">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1851">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1851">Storage</span></span>

* <span data-ttu-id="96718-1852">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="96718-1852">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="96718-1853">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="96718-1853">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="96718-1854">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1854">August 28, 2017</span></span>

<span data-ttu-id="96718-1855">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="96718-1855">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="96718-1856">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="96718-1856">CLI</span></span>

* <span data-ttu-id="96718-1857">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1857">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1858">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1858">ACS</span></span>

* <span data-ttu-id="96718-1859">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1859">Corrected preview regions</span></span>
* <span data-ttu-id="96718-1860">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="96718-1860">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="96718-1861">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="96718-1861">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1862">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1862">Appservice</span></span>

* <span data-ttu-id="96718-1863">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1863">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="96718-1864">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1864">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="96718-1865">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-1865">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="96718-1866">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="96718-1866">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="96718-1867">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="96718-1867">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="96718-1868">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-1868">IoT</span></span>

* <span data-ttu-id="96718-1869">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="96718-1869">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="96718-1870">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1870">Network</span></span>

* <span data-ttu-id="96718-1871">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1871">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="96718-1872">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1872">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="96718-1873">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1873">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="96718-1874">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1874">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="96718-1875">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1875">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1876">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1876">Profile</span></span>

* <span data-ttu-id="96718-1877">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-1877">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="96718-1878">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="96718-1878">Service Fabric</span></span>

* <span data-ttu-id="96718-1879">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="96718-1879">Preview release</span></span>
* <span data-ttu-id="96718-1880">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="96718-1880">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="96718-1881">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1881">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="96718-1882">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1882">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1883">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1883">Storage</span></span>

* <span data-ttu-id="96718-1884">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-1884">Enabled setting blob tier</span></span>
* <span data-ttu-id="96718-1885">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1885">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="96718-1886">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1886">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="96718-1887">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-1887">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="96718-1888">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1888">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="96718-1889">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="96718-1889">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1890">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1890">VM</span></span>

* <span data-ttu-id="96718-1891">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1891">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="96718-1892">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-1892">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="96718-1893">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1893">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="96718-1894">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="96718-1894">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="96718-1895">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1895">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="96718-1896">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-1896">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="96718-1897">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1897">August 15, 2017</span></span>

<span data-ttu-id="96718-1898">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="96718-1898">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1899">ACS</span></span>

* <span data-ttu-id="96718-1900">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-1900">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1901">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1901">Appservice</span></span>

* <span data-ttu-id="96718-1902">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1902">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="96718-1903">Event Grid</span><span class="sxs-lookup"><span data-stu-id="96718-1903">Event Grid</span></span>

* <span data-ttu-id="96718-1904">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1904">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="96718-1905">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1905">August 11, 2017</span></span>

<span data-ttu-id="96718-1906">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="96718-1906">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1907">ACS</span></span>

* <span data-ttu-id="96718-1908">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1908">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1909">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1909">Batch</span></span>

* <span data-ttu-id="96718-1910">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1910">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="96718-1911">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1911">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="96718-1912">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1912">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="96718-1913">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="96718-1913">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="96718-1914">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="96718-1914">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="96718-1915">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1915">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="96718-1916">Komponente</span><span class="sxs-lookup"><span data-stu-id="96718-1916">Component</span></span>

* <span data-ttu-id="96718-1917">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1917">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="96718-1918">Container</span><span class="sxs-lookup"><span data-stu-id="96718-1918">Container</span></span>

* <span data-ttu-id="96718-1919">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="96718-1919">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="96718-1920">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="96718-1920">Data Lake Store</span></span>

* <span data-ttu-id="96718-1921">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-1921">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="96718-1922">Event Grid</span><span class="sxs-lookup"><span data-stu-id="96718-1922">Event Grid</span></span>

* <span data-ttu-id="96718-1923">Erste Version</span><span class="sxs-lookup"><span data-stu-id="96718-1923">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="96718-1924">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-1924">Network</span></span>

* <span data-ttu-id="96718-1925">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="96718-1925">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="96718-1926">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="96718-1926">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="96718-1927">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-1927">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="96718-1928">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="96718-1928">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="96718-1929">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1929">Profile</span></span>

* <span data-ttu-id="96718-1930">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="96718-1930">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="96718-1931">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-1931">Storage</span></span>

* <span data-ttu-id="96718-1932">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-1932">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="96718-1933">VM</span><span class="sxs-lookup"><span data-stu-id="96718-1933">VM</span></span>

* <span data-ttu-id="96718-1934">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-1934">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="96718-1935">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-1935">Exposed `list-skus` command</span></span>
* <span data-ttu-id="96718-1936">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="96718-1936">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="96718-1937">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="96718-1937">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="96718-1938">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-1938">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="96718-1939">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="96718-1939">July 28, 2017</span></span>

<span data-ttu-id="96718-1940">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="96718-1940">Version 2.0.12</span></span>

* <span data-ttu-id="96718-1941">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1941">Added container commands</span></span>
* <span data-ttu-id="96718-1942">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1942">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="96718-1943">Core</span><span class="sxs-lookup"><span data-stu-id="96718-1943">Core</span></span>

* <span data-ttu-id="96718-1944">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="96718-1944">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="96718-1945">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1945">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="96718-1946">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="96718-1946">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="96718-1947">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="96718-1947">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="96718-1948">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="96718-1948">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="96718-1949">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="96718-1949">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="96718-1950">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="96718-1950">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="96718-1951">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="96718-1951">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="96718-1952">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="96718-1952">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="96718-1953">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="96718-1953">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="96718-1954">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="96718-1954">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="96718-1955">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="96718-1955">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="96718-1956">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="96718-1956">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="96718-1957">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="96718-1957">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="96718-1958">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="96718-1958">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="96718-1959">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="96718-1959">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="96718-1960">ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1960">ACR</span></span>

* <span data-ttu-id="96718-1961">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1961">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="96718-1962">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="96718-1962">Support SKU update for managed registries</span></span>
* <span data-ttu-id="96718-1963">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1963">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="96718-1964">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1964">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="96718-1965">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1965">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="96718-1966">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1966">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="96718-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-1967">ACS</span></span>

* <span data-ttu-id="96718-1968">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="96718-1968">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-1969">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-1969">Appservice</span></span>

* <span data-ttu-id="96718-1970">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="96718-1970">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="96718-1971">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="96718-1971">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="96718-1972">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="96718-1972">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="96718-1973">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="96718-1973">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="96718-1974">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="96718-1974">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="96718-1975">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="96718-1975">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="96718-1976">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="96718-1976">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="96718-1977">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="96718-1977">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="96718-1978">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="96718-1978">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="96718-1979">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="96718-1979">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="96718-1980">Batch</span><span class="sxs-lookup"><span data-stu-id="96718-1980">Batch</span></span>

* <span data-ttu-id="96718-1981">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-1981">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="96718-1982">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-1982">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="96718-1983">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1983">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="96718-1984">CDN</span><span class="sxs-lookup"><span data-stu-id="96718-1984">CDN</span></span>

* <span data-ttu-id="96718-1985">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="96718-1985">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="96718-1986">Cloud</span><span class="sxs-lookup"><span data-stu-id="96718-1986">Cloud</span></span>

* <span data-ttu-id="96718-1987">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="96718-1987">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="96718-1988">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="96718-1988">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="96718-1989">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="96718-1989">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="96718-1990">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="96718-1990">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="96718-1991">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="96718-1991">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-1992">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-1992">CosmosDB</span></span>

* <span data-ttu-id="96718-1993">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="96718-1993">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="96718-1994">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1994">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="96718-1995">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="96718-1995">Data Lake Analytics</span></span>

* <span data-ttu-id="96718-1996">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1996">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="96718-1997">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1997">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="96718-1998">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-1998">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="96718-1999">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="96718-1999">Data Lake Store</span></span>

* <span data-ttu-id="96718-2000">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2000">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="96718-2001">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="96718-2001">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="96718-2002">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="96718-2002">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="96718-2003">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="96718-2003">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="96718-2004">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="96718-2004">Interactive</span></span>

* <span data-ttu-id="96718-2005">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-2005">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="96718-2006">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-2006">Increased test coverage</span></span>
* <span data-ttu-id="96718-2007">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="96718-2007">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="96718-2008">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="96718-2008">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="96718-2009">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="96718-2009">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="96718-2010">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="96718-2010">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="96718-2011">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="96718-2011">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="96718-2012">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2012">Added `--progress` flag</span></span>
* <span data-ttu-id="96718-2013">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-2013">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="96718-2014">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="96718-2014">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="96718-2015">IoT</span><span class="sxs-lookup"><span data-stu-id="96718-2015">IoT</span></span>

* <span data-ttu-id="96718-2016">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="96718-2016">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="96718-2017">(3934)</span><span class="sxs-lookup"><span data-stu-id="96718-2017">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="96718-2018">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="96718-2018">Key vault</span></span>

* <span data-ttu-id="96718-2019">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="96718-2019">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="96718-2020">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="96718-2020">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="96718-2021">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="96718-2021">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="96718-2022">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="96718-2022">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="96718-2023">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="96718-2023">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="96718-2024">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="96718-2024">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="96718-2025">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="96718-2025">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="96718-2026">(3307)</span><span class="sxs-lookup"><span data-stu-id="96718-2026">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="96718-2027">Labor</span><span class="sxs-lookup"><span data-stu-id="96718-2027">Lab</span></span>

* <span data-ttu-id="96718-2028">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2028">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="96718-2029">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2029">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-2030">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-2030">Monitor</span></span>

* <span data-ttu-id="96718-2031">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="96718-2031">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="96718-2032">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-2032">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="96718-2033">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-2033">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="96718-2034">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-2034">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="96718-2035">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="96718-2035">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="96718-2036">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="96718-2036">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="96718-2037">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="96718-2037">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="96718-2038">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="96718-2038">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="96718-2039">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="96718-2039">`location` no longer required</span></span>
  * <span data-ttu-id="96718-2040">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="96718-2040">Add name and ID support for target</span></span>
  * <span data-ttu-id="96718-2041">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="96718-2041">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="96718-2042">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="96718-2042">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="96718-2043">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="96718-2043">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="96718-2044">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="96718-2044">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="96718-2045">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="96718-2045">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="96718-2046">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2046">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="96718-2047">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-2047">Network</span></span>

* <span data-ttu-id="96718-2048">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2048">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="96718-2049">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2049">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="96718-2050">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="96718-2050">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="96718-2051">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="96718-2051">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="96718-2052">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="96718-2052">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="96718-2053">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2053">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="96718-2054">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="96718-2054">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="96718-2055">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="96718-2055">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="96718-2056">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="96718-2056">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="96718-2057">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="96718-2057">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="96718-2058">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2058">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="96718-2059">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2059">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="96718-2060">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="96718-2060">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="96718-2061">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2061">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="96718-2062">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2062">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="96718-2063">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-2063">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="96718-2064">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="96718-2064">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="96718-2065">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="96718-2065">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="96718-2066">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2066">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="96718-2067">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-2067">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="96718-2068">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="96718-2068">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="96718-2069">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="96718-2069">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="96718-2070">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-2070">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="96718-2071">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="96718-2071">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="96718-2072">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="96718-2072">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="96718-2073">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="96718-2073">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="96718-2074">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="96718-2074">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="96718-2075">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-2075">Profile</span></span>

* <span data-ttu-id="96718-2076">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="96718-2076">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="96718-2077">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="96718-2077">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="96718-2078">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="96718-2078">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="96718-2079">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2079">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="96718-2080">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="96718-2080">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="96718-2081">RDBMS</span><span class="sxs-lookup"><span data-stu-id="96718-2081">RDBMS</span></span>

* <span data-ttu-id="96718-2082">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="96718-2082">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="96718-2083">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="96718-2083">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="96718-2084">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="96718-2084">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="96718-2085">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="96718-2085">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="96718-2086">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-2086">Resource</span></span>

* <span data-ttu-id="96718-2087">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-2087">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="96718-2088">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="96718-2088">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="96718-2089">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="96718-2089">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="96718-2090">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="96718-2090">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="96718-2091">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="96718-2091">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="96718-2092">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="96718-2092">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="96718-2093">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="96718-2093">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="96718-2094">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2094">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="96718-2095">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-2095">Role</span></span>

* <span data-ttu-id="96718-2096">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="96718-2096">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="96718-2097">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="96718-2097">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="96718-2098">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="96718-2098">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="96718-2099">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="96718-2099">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="96718-2100">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2100">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="96718-2101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="96718-2101">Service Fabric</span></span>
* <span data-ttu-id="96718-2102">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="96718-2102">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="96718-2103">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="96718-2103">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="96718-2104">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="96718-2104">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="96718-2105">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-2105">SQL</span></span>

* <span data-ttu-id="96718-2106">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-2106">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="96718-2107">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="96718-2107">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="96718-2108">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2108">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="96718-2109">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-2109">Storage</span></span>

* <span data-ttu-id="96718-2110">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="96718-2110">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="96718-2111">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="96718-2111">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="96718-2112">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="96718-2112">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="96718-2113">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="96718-2113">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="96718-2114">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="96718-2114">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="96718-2115">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="96718-2115">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="96718-2116">VM</span><span class="sxs-lookup"><span data-stu-id="96718-2116">VM</span></span>

* <span data-ttu-id="96718-2117">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="96718-2117">Support configuring nsg</span></span>
* <span data-ttu-id="96718-2118">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="96718-2118">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="96718-2119">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="96718-2119">Support managed service identities</span></span>
* <span data-ttu-id="96718-2120">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="96718-2120">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="96718-2121">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="96718-2121">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="96718-2122">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="96718-2122">May 10, 2017</span></span>

<span data-ttu-id="96718-2123">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="96718-2123">Version 2.0.6</span></span>

* <span data-ttu-id="96718-2124">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="96718-2124">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="96718-2125">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="96718-2125">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="96718-2126">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="96718-2126">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="96718-2127">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-2127">Include Cognitive Services module</span></span>
* <span data-ttu-id="96718-2128">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-2128">Include Service Fabric module</span></span>
* <span data-ttu-id="96718-2129">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="96718-2129">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="96718-2130">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="96718-2130">Add support for CDN commands</span></span>
* <span data-ttu-id="96718-2131">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="96718-2131">Remove Container module</span></span>
* <span data-ttu-id="96718-2132">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="96718-2132">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="96718-2133">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="96718-2133">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="96718-2134">Core</span><span class="sxs-lookup"><span data-stu-id="96718-2134">Core</span></span>

* <span data-ttu-id="96718-2135">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="96718-2135">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="96718-2136">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="96718-2136">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="96718-2137">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="96718-2137">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="96718-2138">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="96718-2138">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="96718-2139">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="96718-2139">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="96718-2140">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="96718-2140">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="96718-2141">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="96718-2141">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="96718-2142">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="96718-2142">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="96718-2143">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="96718-2143">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="96718-2144">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="96718-2144">core: Improved performance</span></span>
* <span data-ttu-id="96718-2145">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="96718-2145">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="96718-2146">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="96718-2146">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="96718-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-2147">ACS</span></span>

* <span data-ttu-id="96718-2148">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96718-2148">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="96718-2149">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="96718-2149">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="96718-2150">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="96718-2150">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="96718-2151">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="96718-2151">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-2152">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-2152">AppService</span></span>

* <span data-ttu-id="96718-2153">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="96718-2153">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="96718-2154">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="96718-2154">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="96718-2155">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="96718-2155">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="96718-2156">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="96718-2156">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="96718-2157">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="96718-2157">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="96718-2158">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="96718-2158">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="96718-2159">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="96718-2159">support slot swap with preview</span></span>
* <span data-ttu-id="96718-2160">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="96718-2160">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="96718-2161">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="96718-2161">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="96718-2162">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="96718-2162">CosmosDB</span></span>

* <span data-ttu-id="96718-2163">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="96718-2163">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="96718-2164">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="96718-2164">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="96718-2165">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="96718-2165">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="96718-2166">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="96718-2166">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="96718-2167">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="96718-2167">Data Lake Analytics</span></span>

* <span data-ttu-id="96718-2168">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="96718-2168">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="96718-2169">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="96718-2169">Add support for new catalog item type: package.</span></span> <span data-ttu-id="96718-2170">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="96718-2170">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="96718-2171">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="96718-2171">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="96718-2172">Table</span><span class="sxs-lookup"><span data-stu-id="96718-2172">Table</span></span>
  * <span data-ttu-id="96718-2173">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="96718-2173">Table valued function</span></span>
  * <span data-ttu-id="96718-2174">Sicht</span><span class="sxs-lookup"><span data-stu-id="96718-2174">View</span></span>
  * <span data-ttu-id="96718-2175">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="96718-2175">Table Statistics.</span></span> <span data-ttu-id="96718-2176">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="96718-2176">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="96718-2177">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="96718-2177">Data Lake Store</span></span>

* <span data-ttu-id="96718-2178">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="96718-2178">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="96718-2179">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="96718-2179">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="96718-2180">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="96718-2180">missed help for access show.</span></span> <span data-ttu-id="96718-2181">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="96718-2181">adding it.</span></span> <span data-ttu-id="96718-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="96718-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="96718-2183">Suchen</span><span class="sxs-lookup"><span data-stu-id="96718-2183">Find</span></span>

* <span data-ttu-id="96718-2184">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="96718-2184">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="96718-2185">KeyVault</span><span class="sxs-lookup"><span data-stu-id="96718-2185">KeyVault</span></span>

* <span data-ttu-id="96718-2186">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="96718-2186">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="96718-2187">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="96718-2187">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="96718-2188">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="96718-2188">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="96718-2189">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="96718-2189">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="96718-2190">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="96718-2190">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="96718-2191">Labor</span><span class="sxs-lookup"><span data-stu-id="96718-2191">Lab</span></span>

* <span data-ttu-id="96718-2192">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="96718-2192">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="96718-2193">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="96718-2193">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="96718-2194">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="96718-2194">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="96718-2195">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="96718-2195">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="96718-2196">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="96718-2196">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="96718-2197">Überwachen</span><span class="sxs-lookup"><span data-stu-id="96718-2197">Monitor</span></span>

* <span data-ttu-id="96718-2198">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="96718-2198">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="96718-2199">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="96718-2199">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="96718-2200">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-2200">Network</span></span>

* <span data-ttu-id="96718-2201">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="96718-2201">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="96718-2202">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="96718-2202">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="96718-2203">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="96718-2203">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="96718-2204">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="96718-2204">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="96718-2205">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="96718-2205">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="96718-2206">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="96718-2206">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="96718-2207">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="96718-2207">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="96718-2208">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="96718-2208">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="96718-2209">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="96718-2209">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="96718-2210">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="96718-2210">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="96718-2211">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="96718-2211">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="96718-2212">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="96718-2212">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="96718-2213">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="96718-2213">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="96718-2214">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="96718-2214">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="96718-2215">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="96718-2215">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="96718-2216">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="96718-2216">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="96718-2217">Profil</span><span class="sxs-lookup"><span data-stu-id="96718-2217">Profile</span></span>

* <span data-ttu-id="96718-2218">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="96718-2218">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="96718-2219">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="96718-2219">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="96718-2220">Redis</span><span class="sxs-lookup"><span data-stu-id="96718-2220">Redis</span></span>

* <span data-ttu-id="96718-2221">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="96718-2221">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="96718-2222">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="96718-2222">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="96718-2223">Ressource</span><span class="sxs-lookup"><span data-stu-id="96718-2223">Resource</span></span>

* <span data-ttu-id="96718-2224">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="96718-2224">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="96718-2225">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="96718-2225">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="96718-2226">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="96718-2226">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="96718-2227">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="96718-2227">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="96718-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="96718-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="96718-2229">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="96718-2229">Add docs for az lock update.</span></span> <span data-ttu-id="96718-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="96718-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="96718-2231">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="96718-2231">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="96718-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="96718-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="96718-2233">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="96718-2233">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="96718-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="96718-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="96718-2235">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="96718-2235">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="96718-2236">Rolle</span><span class="sxs-lookup"><span data-stu-id="96718-2236">Role</span></span>

* <span data-ttu-id="96718-2237">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="96718-2237">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="96718-2238">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="96718-2238">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="96718-2239">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="96718-2239">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="96718-2240">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="96718-2240">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="96718-2241">SQL</span><span class="sxs-lookup"><span data-stu-id="96718-2241">SQL</span></span>

* <span data-ttu-id="96718-2242">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="96718-2242">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="96718-2243">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="96718-2243">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="96718-2244">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-2244">Storage</span></span>

* <span data-ttu-id="96718-2245">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="96718-2245">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="96718-2246">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="96718-2246">Add support for incremental blob copy</span></span>
* <span data-ttu-id="96718-2247">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="96718-2247">Add support for large block blob upload</span></span>
* <span data-ttu-id="96718-2248">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="96718-2248">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="96718-2249">VM</span><span class="sxs-lookup"><span data-stu-id="96718-2249">VM</span></span>

* <span data-ttu-id="96718-2250">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="96718-2250">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="96718-2251">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="96718-2251">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="96718-2252">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="96718-2252">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="96718-2253">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="96718-2253">az vm/vmss disk</span></span>
  3. <span data-ttu-id="96718-2254">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="96718-2254">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="96718-2255">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="96718-2255">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="96718-2256">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="96718-2256">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="96718-2257">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="96718-2257">April 3, 2017</span></span>

<span data-ttu-id="96718-2258">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="96718-2258">Version 2.0.2</span></span>

<span data-ttu-id="96718-2259">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="96718-2259">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="96718-2260">Core</span><span class="sxs-lookup"><span data-stu-id="96718-2260">Core</span></span>

* <span data-ttu-id="96718-2261">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="96718-2261">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="96718-2262">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="96718-2262">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="96718-2263">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="96718-2263">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="96718-2264">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="96718-2264">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="96718-2265">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="96718-2265">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="96718-2266">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="96718-2266">Add prompting for missing template parameters.</span></span> <span data-ttu-id="96718-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="96718-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="96718-2268">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="96718-2268">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="96718-2269">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="96718-2269">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="96718-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="96718-2270">ACS</span></span>

* <span data-ttu-id="96718-2271">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="96718-2271">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="96718-2272">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="96718-2272">Add support for ssh key password prompting.</span></span> <span data-ttu-id="96718-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="96718-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="96718-2274">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="96718-2274">Add support for windows clusters.</span></span> <span data-ttu-id="96718-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="96718-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="96718-2276">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="96718-2276">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="96718-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="96718-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="96718-2278">AppService</span><span class="sxs-lookup"><span data-stu-id="96718-2278">AppService</span></span>

* <span data-ttu-id="96718-2279">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="96718-2279">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="96718-2280">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="96718-2280">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="96718-2281">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="96718-2281">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="96718-2282">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="96718-2282">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="96718-2283">DataLake</span><span class="sxs-lookup"><span data-stu-id="96718-2283">DataLake</span></span>

* <span data-ttu-id="96718-2284">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-2284">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="96718-2285">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="96718-2285">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="96718-2286">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="96718-2286">DocuemntDB</span></span>

* <span data-ttu-id="96718-2287">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="96718-2287">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="96718-2288">VM</span><span class="sxs-lookup"><span data-stu-id="96718-2288">VM</span></span>

* <span data-ttu-id="96718-2289">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="96718-2289">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="96718-2290">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="96718-2290">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="96718-2291">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="96718-2291">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="96718-2292">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="96718-2292">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="96718-2293">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="96718-2293">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="96718-2294">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="96718-2294">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="96718-2295">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="96718-2295">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="96718-2296">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="96718-2296">February 27, 2017</span></span>

<span data-ttu-id="96718-2297">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="96718-2297">Version 2.0.0</span></span>

<span data-ttu-id="96718-2298">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="96718-2298">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="96718-2299">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="96718-2299">Container Service (acs)</span></span>
- <span data-ttu-id="96718-2300">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="96718-2300">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="96718-2301">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="96718-2301">Networking</span></span>
- <span data-ttu-id="96718-2302">Storage</span><span class="sxs-lookup"><span data-stu-id="96718-2302">Storage</span></span>

<span data-ttu-id="96718-2303">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="96718-2303">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="96718-2304">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="96718-2304">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="96718-2305">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="96718-2305">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="96718-2306">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="96718-2306">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="96718-2307">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="96718-2307">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="96718-2308">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="96718-2308">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="96718-2309">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="96718-2309">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="96718-2310">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="96718-2310">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="96718-2311">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="96718-2311">Provide feedback from the command line with the `az feedback` command</span></span>


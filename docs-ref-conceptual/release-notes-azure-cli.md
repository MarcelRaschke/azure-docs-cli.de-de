---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/18/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 10663ad8e85a15b8fedb5ac12c5d17256d07e523
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805957"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="32b2a-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="32b2a-103">Azure CLI release notes</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="32b2a-104">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-104">December 20, 2018</span></span>

<span data-ttu-id="32b2a-105">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="32b2a-105">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="32b2a-106">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-106">Appservice</span></span>
* <span data-ttu-id="32b2a-107">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-107">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="32b2a-108">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-108">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="32b2a-109">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-109">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="32b2a-110">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="32b2a-110">IoTCentral</span></span>
* <span data-ttu-id="32b2a-111">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-111">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-112">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-112">Role</span></span>
* <span data-ttu-id="32b2a-113">[WICHTIGE ÄNDERUNG] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-113">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-114">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-114">SQL</span></span>
* <span data-ttu-id="32b2a-115">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-115">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-116">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-116">VM</span></span>
* <span data-ttu-id="32b2a-117">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-117">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="32b2a-118">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-118">December 18, 2018</span></span>

<span data-ttu-id="32b2a-119">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="32b2a-119">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="32b2a-120">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-120">ACR</span></span>
* <span data-ttu-id="32b2a-121">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-121">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="32b2a-122">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-122">Condensed the table layout for task list</span></span>
* <span data-ttu-id="32b2a-123">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-123">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-124">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-124">ACS</span></span>
* <span data-ttu-id="32b2a-125">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-125">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="32b2a-126">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-126">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="32b2a-127">[VERALTET] `az acs`-Befehle als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="32b2a-127">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="32b2a-128">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="32b2a-128">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="32b2a-129">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-129">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="32b2a-130">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-130">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-131">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-131">Appservice</span></span>
* <span data-ttu-id="32b2a-132">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-132">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="32b2a-133">Botservice</span><span class="sxs-lookup"><span data-stu-id="32b2a-133">Botservice</span></span>
* <span data-ttu-id="32b2a-134">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-134">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="32b2a-135">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-135">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="32b2a-136">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-136">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="32b2a-137">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="32b2a-137">Reduced Kudu network calls</span></span>
* <span data-ttu-id="32b2a-138">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="32b2a-138">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-139">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-139">Consumption</span></span>
* <span data-ttu-id="32b2a-140">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-140">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-141">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-141">CosmosDB</span></span>
* <span data-ttu-id="32b2a-142">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-142">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="32b2a-143">Karten</span><span class="sxs-lookup"><span data-stu-id="32b2a-143">Maps</span></span>
* <span data-ttu-id="32b2a-144">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-144">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-145">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-145">Network</span></span>
* <span data-ttu-id="32b2a-146">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-146">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="32b2a-147">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="32b2a-147">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-148">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-148">Resource</span></span>
* <span data-ttu-id="32b2a-149">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-149">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="32b2a-150">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-150">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-151">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-151">Storage</span></span>
*  <span data-ttu-id="32b2a-152">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-152">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-153">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-153">VM</span></span>
* <span data-ttu-id="32b2a-154">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="32b2a-154">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="32b2a-155">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-155">December 4, 2018</span></span>

<span data-ttu-id="32b2a-156">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="32b2a-156">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="32b2a-157">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-157">Core</span></span>
* <span data-ttu-id="32b2a-158">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-158">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="32b2a-159">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-159">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-160">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-160">Appservice</span></span>
* <span data-ttu-id="32b2a-161">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="32b2a-161">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="32b2a-162">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="32b2a-162">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-163">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-163">Network</span></span>
* <span data-ttu-id="32b2a-164">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-164">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-165">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-165">Role</span></span>
* <span data-ttu-id="32b2a-166">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-166">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="32b2a-167">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-167">VM</span></span>
* <span data-ttu-id="32b2a-168">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-168">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="32b2a-169">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="32b2a-169">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="32b2a-170">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="32b2a-170">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="32b2a-171">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="32b2a-171">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="32b2a-172">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-172">November 20, 2018</span></span>

<span data-ttu-id="32b2a-173">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="32b2a-173">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="32b2a-174">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-174">Core</span></span>
* <span data-ttu-id="32b2a-175">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-175">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-176">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-176">ACR</span></span>
* <span data-ttu-id="32b2a-177">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-177">Added context token to task step</span></span>
* <span data-ttu-id="32b2a-178">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-178">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="32b2a-179">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-179">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-180">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-180">Appservice</span></span>
* <span data-ttu-id="32b2a-181">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-181">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="32b2a-182">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-182">Updated the default `node_version`.</span></span> <span data-ttu-id="32b2a-183">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="32b2a-183">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="32b2a-184">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-184">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="32b2a-185">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="32b2a-185">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="32b2a-186">IotCentral</span><span class="sxs-lookup"><span data-stu-id="32b2a-186">IotCentral</span></span>
* <span data-ttu-id="32b2a-187">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-187">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-188">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-188">KeyVault</span></span>
* <span data-ttu-id="32b2a-189">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-189">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-190">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-190">Network</span></span>
* <span data-ttu-id="32b2a-191">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-191">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="32b2a-192">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-192">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="32b2a-193">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-193">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="32b2a-194">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-194">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-195">Rdbms</span><span class="sxs-lookup"><span data-stu-id="32b2a-195">Rdbms</span></span>
* <span data-ttu-id="32b2a-196">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-196">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="32b2a-197">RBAC</span><span class="sxs-lookup"><span data-stu-id="32b2a-197">Rbac</span></span>
* <span data-ttu-id="32b2a-198">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-198">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="32b2a-199">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-199">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="32b2a-200">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-200">Storage</span></span>
* <span data-ttu-id="32b2a-201">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-201">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="32b2a-202">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="32b2a-202">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="32b2a-203">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-203">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="32b2a-204">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-204">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-205">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-205">VM</span></span>
* <span data-ttu-id="32b2a-206">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-206">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="32b2a-207">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-207">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="32b2a-208">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="32b2a-208">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="32b2a-209">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-209">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="32b2a-210">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-210">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="32b2a-211">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-211">Added `snapshot wait` command</span></span>
* <span data-ttu-id="32b2a-212">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-212">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="32b2a-213">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-213">November 6, 2018</span></span>

<span data-ttu-id="32b2a-214">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="32b2a-214">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-215">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-215">Core</span></span>
* <span data-ttu-id="32b2a-216">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-216">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-217">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-217">ACR</span></span>
* <span data-ttu-id="32b2a-218">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-218">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="32b2a-219">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-219">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-220">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-220">ACS</span></span>
* <span data-ttu-id="32b2a-221">[WICHTIGE ÄNDERUNG] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-221">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="32b2a-222">Advisor</span><span class="sxs-lookup"><span data-stu-id="32b2a-222">Advisor</span></span>
* <span data-ttu-id="32b2a-223">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="32b2a-223">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="32b2a-224">AMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-224">AMS</span></span>
* <span data-ttu-id="32b2a-225">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-225">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="32b2a-226">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-226">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="32b2a-227">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-227">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="32b2a-228">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-228">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="32b2a-229">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-229">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="32b2a-230">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-230">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="32b2a-231">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-231">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="32b2a-232">[WICHTIGE ÄNDERUNG] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="32b2a-232">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="32b2a-233">[WICHTIGE ÄNDERUNG] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-233">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="32b2a-234">[WICHTIGE ÄNDERUNG] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-234">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="32b2a-235">[WICHTIGE ÄNDERUNG] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="32b2a-235">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="32b2a-236">[WICHTIGE ÄNDERUNG] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-236">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="32b2a-237">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="32b2a-237">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="32b2a-238">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-238">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="32b2a-239">[WICHTIGE ÄNDERUNG] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-239">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="32b2a-240">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-240">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="32b2a-241">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="32b2a-241">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-242">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-242">AppService</span></span>
* <span data-ttu-id="32b2a-243">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="32b2a-243">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="32b2a-244">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-244">Configure</span></span>
* <span data-ttu-id="32b2a-245">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-245">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-246">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-246">Container</span></span>
* <span data-ttu-id="32b2a-247">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-247">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="32b2a-248">EventHub</span><span class="sxs-lookup"><span data-stu-id="32b2a-248">EventHub</span></span>
* <span data-ttu-id="32b2a-249">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-249">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-250">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-250">Interactive</span></span>
* <span data-ttu-id="32b2a-251">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-251">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-252">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-252">Monitor</span></span>
* <span data-ttu-id="32b2a-253">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-253">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-254">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-254">Network</span></span>
* <span data-ttu-id="32b2a-255">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-255">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="32b2a-256">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-256">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="32b2a-257">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="32b2a-257">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="32b2a-258">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-258">Profile</span></span>
* <span data-ttu-id="32b2a-259">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-259">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-260">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-260">RDBMS</span></span>
* <span data-ttu-id="32b2a-261">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-261">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-262">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-262">Resource</span></span>
* <span data-ttu-id="32b2a-263">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-263">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-264">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-264">Role</span></span>
* <span data-ttu-id="32b2a-265">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-265">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="32b2a-266">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="32b2a-266">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="32b2a-267">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-267">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-268">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-268">Storage</span></span>
* <span data-ttu-id="32b2a-269">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="32b2a-269">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-270">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-270">VM</span></span>
* <span data-ttu-id="32b2a-271">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-271">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="32b2a-272">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="32b2a-272">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="32b2a-273">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-273">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="32b2a-274">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-274">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="32b2a-275">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="32b2a-275">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="32b2a-276">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-276">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="32b2a-277">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-277">October 23, 2018</span></span>

<span data-ttu-id="32b2a-278">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="32b2a-278">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-279">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-279">Core</span></span>
* <span data-ttu-id="32b2a-280">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="32b2a-280">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="32b2a-281">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="32b2a-281">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-282">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-282">ACR</span></span>
* <span data-ttu-id="32b2a-283">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-283">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="32b2a-284">CDN</span><span class="sxs-lookup"><span data-stu-id="32b2a-284">CDN</span></span>
* <span data-ttu-id="32b2a-285">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="32b2a-285">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="32b2a-286">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-286">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-287">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-287">Container</span></span>
* <span data-ttu-id="32b2a-288">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-288">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="32b2a-289">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-289">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="32b2a-290">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-290">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="32b2a-291">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="32b2a-291">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="32b2a-292">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="32b2a-292">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="32b2a-293">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-293">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="32b2a-294">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-294">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-295">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-295">CosmosDB</span></span>
* <span data-ttu-id="32b2a-296">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-296">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-297">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-297">Interactive</span></span>
* <span data-ttu-id="32b2a-298">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-298">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="32b2a-299">IoT Central</span><span class="sxs-lookup"><span data-stu-id="32b2a-299">IoT Central</span></span>
* <span data-ttu-id="32b2a-300">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-300">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="32b2a-301">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-301">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-302">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-302">Monitor</span></span>
* <span data-ttu-id="32b2a-303">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="32b2a-303">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="32b2a-304">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-304">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="32b2a-305">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-305">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="32b2a-306">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-306">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="32b2a-307">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-307">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="32b2a-308">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-308">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="32b2a-309">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="32b2a-309">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="32b2a-310">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-310">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="32b2a-311">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-311">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="32b2a-312">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-312">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-313">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-313">Network</span></span>
* <span data-ttu-id="32b2a-314">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-314">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="32b2a-315">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-315">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="32b2a-316">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32b2a-316">ServiceBus</span></span>
* <span data-ttu-id="32b2a-317">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-317">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-318">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-318">SQL</span></span>
* <span data-ttu-id="32b2a-319">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-319">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-320">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-320">Storage</span></span>
* <span data-ttu-id="32b2a-321">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-321">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="32b2a-322">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-322">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-323">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-323">VM</span></span>
* <span data-ttu-id="32b2a-324">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-324">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="32b2a-325">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-325">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="32b2a-326">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-326">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="32b2a-327">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-327">October 16, 2018</span></span>

<span data-ttu-id="32b2a-328">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="32b2a-328">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-329">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-329">VM</span></span>
* <span data-ttu-id="32b2a-330">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-330">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="32b2a-331">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-331">October 9, 2018</span></span>

<span data-ttu-id="32b2a-332">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="32b2a-332">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-333">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-333">Core</span></span>
* <span data-ttu-id="32b2a-334">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="32b2a-334">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-335">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-335">ACR</span></span>
* <span data-ttu-id="32b2a-336">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-336">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-337">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-337">ACS</span></span>
* <span data-ttu-id="32b2a-338">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="32b2a-338">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="32b2a-339">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="32b2a-339">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="32b2a-340">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-340">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="32b2a-341">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="32b2a-341">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-342">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-342">Container</span></span>
* <span data-ttu-id="32b2a-343">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-343">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="32b2a-344">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-344">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="32b2a-345">Event Hub</span><span class="sxs-lookup"><span data-stu-id="32b2a-345">Event Hub</span></span>
* <span data-ttu-id="32b2a-346">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-346">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="32b2a-347">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-347">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="32b2a-348">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-348">Extensions</span></span>
* <span data-ttu-id="32b2a-349">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-349">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="32b2a-350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="32b2a-350">HDInsight</span></span>
* <span data-ttu-id="32b2a-351">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-351">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-352">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-352">IoT</span></span>
* <span data-ttu-id="32b2a-353">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-353">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-354">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-354">KeyVault</span></span>
* <span data-ttu-id="32b2a-355">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="32b2a-355">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-356">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-356">Network</span></span>
* <span data-ttu-id="32b2a-357">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="32b2a-357">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="32b2a-358">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="32b2a-358">See #6052</span></span>
* <span data-ttu-id="32b2a-359">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="32b2a-359">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="32b2a-360">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-360">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="32b2a-361">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-361">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="32b2a-362">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-362">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="32b2a-363">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-363">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="32b2a-364">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-364">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-365">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-365">Role</span></span>
* <span data-ttu-id="32b2a-366">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-366">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="32b2a-367">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-367">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="32b2a-368">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-368">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="32b2a-369">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-369">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="32b2a-370">Service Bus</span><span class="sxs-lookup"><span data-stu-id="32b2a-370">Service Bus</span></span>
* <span data-ttu-id="32b2a-371">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-371">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-372">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-372">VM</span></span>
* <span data-ttu-id="32b2a-373">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-373">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="32b2a-374">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-374">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="32b2a-375">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-375">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="32b2a-376">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-376">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="32b2a-377">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-377">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="32b2a-378">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-378">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="32b2a-379">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-379">September 21, 2018</span></span>

<span data-ttu-id="32b2a-380">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="32b2a-380">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-381">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-381">ACR</span></span>
* <span data-ttu-id="32b2a-382">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-382">Added ACR Task commands</span></span>
* <span data-ttu-id="32b2a-383">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-383">Added quick run command</span></span>
* <span data-ttu-id="32b2a-384">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-384">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="32b2a-385">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-385">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="32b2a-386">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-386">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="32b2a-387">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-387">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-388">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-388">ACS</span></span>
* <span data-ttu-id="32b2a-389">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-389">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="32b2a-390">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-390">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-391">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-391">AppService</span></span>

* <span data-ttu-id="32b2a-392">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="32b2a-392">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="32b2a-393">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-393">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="32b2a-394">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-394">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="32b2a-395">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-395">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-396">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-396">Batch</span></span>
* <span data-ttu-id="32b2a-397">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-397">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="32b2a-398">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-398">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="32b2a-399">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-399">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="32b2a-400">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-400">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="32b2a-401">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-401">Batch AI</span></span> 
* <span data-ttu-id="32b2a-402">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-402">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="32b2a-403">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="32b2a-403">Cognitive Services</span></span>
* <span data-ttu-id="32b2a-404">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-404">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="32b2a-405">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-405">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="32b2a-406">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-406">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="32b2a-407">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-407">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="32b2a-408">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-408">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="32b2a-409">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="32b2a-409">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-410">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-410">Container</span></span>
* <span data-ttu-id="32b2a-411">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-411">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="32b2a-412">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-412">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="32b2a-413">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-413">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="32b2a-414">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-414">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="32b2a-415">Data Lake</span><span class="sxs-lookup"><span data-stu-id="32b2a-415">Datalake</span></span>
* <span data-ttu-id="32b2a-416">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-416">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="32b2a-417">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="32b2a-417">Interactive Shell</span></span>
* <span data-ttu-id="32b2a-418">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-418">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="32b2a-419">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-419">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-420">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-420">IoT</span></span>
* <span data-ttu-id="32b2a-421">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-421">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="32b2a-422">Key Vault</span><span class="sxs-lookup"><span data-stu-id="32b2a-422">Key Vault</span></span>
* <span data-ttu-id="32b2a-423">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-423">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-424">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-424">Network</span></span>
* <span data-ttu-id="32b2a-425">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-425">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="32b2a-426">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-426">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="32b2a-427">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-427">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="32b2a-428">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-428">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="32b2a-429">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-429">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="32b2a-430">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-430">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="32b2a-431">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-431">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="32b2a-432">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="32b2a-432">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="32b2a-433">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-433">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="32b2a-434">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-434">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="32b2a-435">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-435">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="32b2a-436">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-436">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="32b2a-437">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-437">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="32b2a-438">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="32b2a-438">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="32b2a-439">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-439">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="32b2a-440">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="32b2a-440">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="32b2a-441">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-441">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="32b2a-442">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-442">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-443">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-443">RDBMS</span></span>
* <span data-ttu-id="32b2a-444">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-444">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="32b2a-445">Reservierung</span><span class="sxs-lookup"><span data-stu-id="32b2a-445">Reservation</span></span>
* <span data-ttu-id="32b2a-446">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-446">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="32b2a-447">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-447">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="32b2a-448">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="32b2a-448">Manage App</span></span>
* <span data-ttu-id="32b2a-449">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="32b2a-449">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="32b2a-450">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="32b2a-450">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-451">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-451">Role</span></span>
* <span data-ttu-id="32b2a-452">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-452">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="32b2a-453">SignalR</span><span class="sxs-lookup"><span data-stu-id="32b2a-453">SignalR</span></span>
* <span data-ttu-id="32b2a-454">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-454">First release</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-455">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-455">Storage</span></span>
* <span data-ttu-id="32b2a-456">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-456">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="32b2a-457">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-457">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-458">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-458">VM</span></span>
* <span data-ttu-id="32b2a-459">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="32b2a-459">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="32b2a-460">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-460">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="32b2a-461">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-461">August 28, 2018</span></span>

<span data-ttu-id="32b2a-462">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="32b2a-462">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-463">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-463">Core</span></span>

* <span data-ttu-id="32b2a-464">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-464">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="32b2a-465">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-465">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-466">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-466">ACR</span></span>

* <span data-ttu-id="32b2a-467">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-467">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="32b2a-468">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="32b2a-468">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-469">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-469">ACS</span></span>

* <span data-ttu-id="32b2a-470">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-470">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="32b2a-471">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="32b2a-471">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-472">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-472">AppService</span></span>

* <span data-ttu-id="32b2a-473">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-473">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="32b2a-474">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-474">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="32b2a-475">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-475">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="32b2a-476">Backup</span><span class="sxs-lookup"><span data-stu-id="32b2a-476">Backup</span></span>

* <span data-ttu-id="32b2a-477">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-477">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="32b2a-478">Botdienst</span><span class="sxs-lookup"><span data-stu-id="32b2a-478">Bot Service</span></span>

* <span data-ttu-id="32b2a-479">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="32b2a-479">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="32b2a-480">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="32b2a-480">Cognitive Services</span></span>

* <span data-ttu-id="32b2a-481">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-481">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-482">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-482">IoT</span></span>

* <span data-ttu-id="32b2a-483">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-483">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-484">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-484">Monitor</span></span>

* <span data-ttu-id="32b2a-485">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-485">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="32b2a-486">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-486">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-487">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-487">Network</span></span>

* <span data-ttu-id="32b2a-488">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-488">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-489">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-489">Resource</span></span>

* <span data-ttu-id="32b2a-490">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-490">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-491">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-491">Storage</span></span>

* <span data-ttu-id="32b2a-492">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-492">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-493">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-493">VM</span></span>

* <span data-ttu-id="32b2a-494">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-494">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="32b2a-495">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="32b2a-495">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="32b2a-496">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-496">Auguest 14, 2018</span></span>

<span data-ttu-id="32b2a-497">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="32b2a-497">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-498">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-498">Core</span></span>

* <span data-ttu-id="32b2a-499">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-499">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="32b2a-500">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-500">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="32b2a-501">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="32b2a-501">Telemetry</span></span>

* <span data-ttu-id="32b2a-502">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="32b2a-502">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-503">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-503">ACR</span></span>

* <span data-ttu-id="32b2a-504">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-504">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="32b2a-505">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-505">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-506">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-506">ACS</span></span>

* <span data-ttu-id="32b2a-507">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-507">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="32b2a-508">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-508">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="32b2a-509">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="32b2a-509">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="32b2a-510">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-510">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="32b2a-511">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-511">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="32b2a-512">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-512">AppService</span></span>

* <span data-ttu-id="32b2a-513">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="32b2a-513">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="32b2a-514">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-514">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="32b2a-515">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-515">BatchAI</span></span>

* <span data-ttu-id="32b2a-516">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-516">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="32b2a-517">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-517">Container</span></span>

* <span data-ttu-id="32b2a-518">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-518">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="32b2a-519">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-519">IoT</span></span>

* <span data-ttu-id="32b2a-520">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-520">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="32b2a-521">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="32b2a-521">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="32b2a-522">Iot Central</span><span class="sxs-lookup"><span data-stu-id="32b2a-522">Iot Central</span></span>

* <span data-ttu-id="32b2a-523">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-523">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-524">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-524">KeyVault</span></span>


* <span data-ttu-id="32b2a-525">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-525">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="32b2a-526">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-526">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="32b2a-527">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-527">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="32b2a-528">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-528">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="32b2a-529">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-529">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="32b2a-530">Relay</span><span class="sxs-lookup"><span data-stu-id="32b2a-530">Relay</span></span>

* <span data-ttu-id="32b2a-531">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-531">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-532">Sql</span><span class="sxs-lookup"><span data-stu-id="32b2a-532">Sql</span></span>

* <span data-ttu-id="32b2a-533">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-533">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-534">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-534">Storage</span></span>

* <span data-ttu-id="32b2a-535">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="32b2a-535">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="32b2a-536">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-536">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="32b2a-537">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-537">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="32b2a-538">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-538">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="32b2a-539">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="32b2a-539">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-540">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-540">VM</span></span>

* <span data-ttu-id="32b2a-541">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-541">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="32b2a-542">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-542">July 31, 2018</span></span>

<span data-ttu-id="32b2a-543">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="32b2a-543">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-544">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-544">ACR</span></span>

* <span data-ttu-id="32b2a-545">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-545">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="32b2a-546">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-546">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-547">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-547">ACS</span></span>

* <span data-ttu-id="32b2a-548">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-548">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-549">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-549">Batch</span></span>

* <span data-ttu-id="32b2a-550">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="32b2a-550">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-551">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-551">Container</span></span>

* <span data-ttu-id="32b2a-552">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-552">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-553">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-553">Network</span></span>

* <span data-ttu-id="32b2a-554">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-554">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="32b2a-555">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-555">Resource</span></span>

* <span data-ttu-id="32b2a-556">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="32b2a-556">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="32b2a-557">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="32b2a-557">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-558">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-558">Role</span></span>

* <span data-ttu-id="32b2a-559">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-559">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="32b2a-560">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="32b2a-560">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="32b2a-561">Suchen,</span><span class="sxs-lookup"><span data-stu-id="32b2a-561">Search</span></span>

* <span data-ttu-id="32b2a-562">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-562">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="32b2a-563">Service Bus</span><span class="sxs-lookup"><span data-stu-id="32b2a-563">Service Bus</span></span>

* <span data-ttu-id="32b2a-564">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-564">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="32b2a-565">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-565">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="32b2a-566">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="32b2a-566">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="32b2a-567">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="32b2a-567">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-568">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-568">Storage</span></span>

* <span data-ttu-id="32b2a-569">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-569">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="32b2a-570">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-570">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-571">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-571">VM</span></span>

* <span data-ttu-id="32b2a-572">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-572">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="32b2a-573">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-573">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="32b2a-574">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-574">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="32b2a-575">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-575">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="32b2a-576">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-576">July 18, 2018</span></span>

<span data-ttu-id="32b2a-577">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="32b2a-577">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-578">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-578">Core</span></span>

* <span data-ttu-id="32b2a-579">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-579">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="32b2a-580">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-580">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="32b2a-581">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="32b2a-581">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-582">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-582">ACR</span></span>

* <span data-ttu-id="32b2a-583">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-583">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="32b2a-584">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-584">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="32b2a-585">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-585">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="32b2a-586">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-586">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-587">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-587">ACS</span></span>

* <span data-ttu-id="32b2a-588">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-588">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-589">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-589">AppService</span></span>

* <span data-ttu-id="32b2a-590">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-590">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-591">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-591">Batch</span></span>

* <span data-ttu-id="32b2a-592">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="32b2a-592">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="32b2a-593">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-593">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="32b2a-594">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-594">Batch AI</span></span>

* <span data-ttu-id="32b2a-595">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-595">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-596">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-596">Container</span></span>

* <span data-ttu-id="32b2a-597">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-597">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="32b2a-598">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-598">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-599">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-599">Network</span></span>

* <span data-ttu-id="32b2a-600">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-600">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="32b2a-601">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-601">Added `network nic wait`</span></span>
* <span data-ttu-id="32b2a-602">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-602">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="32b2a-603">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="32b2a-603">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="32b2a-604">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-604">Resource</span></span>

* <span data-ttu-id="32b2a-605">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-605">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="32b2a-606">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-606">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="32b2a-607">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-607">Added `deployment wait` command</span></span>
* <span data-ttu-id="32b2a-608">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-608">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-609">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-609">SQL</span></span>

* <span data-ttu-id="32b2a-610">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-610">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="32b2a-611">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="32b2a-611">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="32b2a-612">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-612">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-613">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-613">Storage</span></span>

* <span data-ttu-id="32b2a-614">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-614">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-615">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-615">VM</span></span>

* <span data-ttu-id="32b2a-616">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-616">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="32b2a-617">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-617">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="32b2a-618">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-618">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="32b2a-619">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-619">July 3, 2018</span></span>

<span data-ttu-id="32b2a-620">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="32b2a-620">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="32b2a-621">AKS</span><span class="sxs-lookup"><span data-stu-id="32b2a-621">AKS</span></span>

* <span data-ttu-id="32b2a-622">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-622">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="32b2a-623">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-623">July 3, 2018</span></span>

<span data-ttu-id="32b2a-624">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="32b2a-624">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-625">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-625">Core</span></span>

* <span data-ttu-id="32b2a-626">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-626">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-627">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-627">ACR</span></span>

* <span data-ttu-id="32b2a-628">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-628">Added polling build status</span></span>
* <span data-ttu-id="32b2a-629">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-629">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="32b2a-630">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-630">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-631">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-631">ACS</span></span>

* <span data-ttu-id="32b2a-632">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="32b2a-632">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="32b2a-633">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-633">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="32b2a-634">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-634">Updated options for `aks browse` command.</span></span> <span data-ttu-id="32b2a-635">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-635">Added `--listen-port` support</span></span>
* <span data-ttu-id="32b2a-636">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-636">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="32b2a-637">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="32b2a-637">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="32b2a-638">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-638">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-639">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-639">AppService</span></span>

* <span data-ttu-id="32b2a-640">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-640">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="32b2a-641">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-641">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="32b2a-642">Backup</span><span class="sxs-lookup"><span data-stu-id="32b2a-642">Backup</span></span>

* <span data-ttu-id="32b2a-643">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-643">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="32b2a-644">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-644">BatchAI</span></span>

* <span data-ttu-id="32b2a-645">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-645">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="32b2a-646">Cloud</span><span class="sxs-lookup"><span data-stu-id="32b2a-646">Cloud</span></span>

* <span data-ttu-id="32b2a-647">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-647">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-648">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-648">Container</span></span>

* <span data-ttu-id="32b2a-649">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-649">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="32b2a-650">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-650">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="32b2a-651">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-651">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-652">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-652">Extension</span></span>

* <span data-ttu-id="32b2a-653">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-653">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-654">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-654">Network</span></span>

* <span data-ttu-id="32b2a-655">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="32b2a-655">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-656">Rdbms</span><span class="sxs-lookup"><span data-stu-id="32b2a-656">Rdbms</span></span>

* <span data-ttu-id="32b2a-657">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-657">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-658">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-658">Resource</span></span>

* <span data-ttu-id="32b2a-659">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-659">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-660">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-660">VM</span></span>

* <span data-ttu-id="32b2a-661">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-661">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="32b2a-662">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-662">June 25, 2018</span></span>

<span data-ttu-id="32b2a-663">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="32b2a-663">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="32b2a-664">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="32b2a-664">CLI</span></span>

* <span data-ttu-id="32b2a-665">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="32b2a-665">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="32b2a-666">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-666">June 19, 2018</span></span>

<span data-ttu-id="32b2a-667">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="32b2a-667">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-668">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-668">Core</span></span>

* <span data-ttu-id="32b2a-669">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-669">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-670">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-670">ACR</span></span>

* <span data-ttu-id="32b2a-671">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-671">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="32b2a-672">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-672">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-673">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-673">ACS</span></span>

* <span data-ttu-id="32b2a-674">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-674">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="32b2a-675">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-675">Added `--update` support</span></span>
* <span data-ttu-id="32b2a-676">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-676">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="32b2a-677">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-677">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="32b2a-678">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-678">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="32b2a-679">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="32b2a-679">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="32b2a-680">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-680">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="32b2a-681">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-681">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-682">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-682">AppService</span></span>

* <span data-ttu-id="32b2a-683">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-683">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="32b2a-684">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-684">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-685">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-685">Batch</span></span>

* <span data-ttu-id="32b2a-686">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-686">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="32b2a-687">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-687">Batch AI</span></span>

* <span data-ttu-id="32b2a-688">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-688">Added support for workspaces.</span></span> <span data-ttu-id="32b2a-689">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="32b2a-689">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="32b2a-690">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-690">Added support for experiments.</span></span> <span data-ttu-id="32b2a-691">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-691">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="32b2a-692">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-692">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="32b2a-693">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-693">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="32b2a-694">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="32b2a-694">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="32b2a-695">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-695">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="32b2a-696">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-696">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="32b2a-697">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-697">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="32b2a-698">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-698">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="32b2a-699">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="32b2a-699">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="32b2a-700">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-700">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="32b2a-701">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="32b2a-701">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="32b2a-702">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-702">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="32b2a-703">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="32b2a-703">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="32b2a-704">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-704">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="32b2a-705">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="32b2a-705">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="32b2a-706">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-706">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="32b2a-707">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-707">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="32b2a-708">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-708">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="32b2a-709">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-709">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="32b2a-710">Karten</span><span class="sxs-lookup"><span data-stu-id="32b2a-710">Maps</span></span>

* <span data-ttu-id="32b2a-711">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-711">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-712">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-712">Network</span></span>

* <span data-ttu-id="32b2a-713">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="32b2a-713">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="32b2a-714">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="32b2a-714">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="32b2a-715">#6502</span><span class="sxs-lookup"><span data-stu-id="32b2a-715">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="32b2a-716">Reservations</span><span class="sxs-lookup"><span data-stu-id="32b2a-716">Reservations</span></span>

* <span data-ttu-id="32b2a-717">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-717">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="32b2a-718">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-718">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="32b2a-719">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-719">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="32b2a-720">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-720">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="32b2a-721">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-721">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="32b2a-722">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-722">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-723">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-723">Role</span></span>

* <span data-ttu-id="32b2a-724">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-724">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-725">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-725">SQL</span></span>

* <span data-ttu-id="32b2a-726">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-726">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-727">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-727">Storage</span></span>

* <span data-ttu-id="32b2a-728">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-728">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-729">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-729">VM</span></span>

* <span data-ttu-id="32b2a-730">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="32b2a-730">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="32b2a-731">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-731">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="32b2a-732">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-732">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="32b2a-733">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-733">June 13, 2018</span></span>

<span data-ttu-id="32b2a-734">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="32b2a-734">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-735">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-735">Core</span></span>

* <span data-ttu-id="32b2a-736">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="32b2a-736">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="32b2a-737">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-737">June 13, 2018</span></span>

<span data-ttu-id="32b2a-738">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="32b2a-738">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="32b2a-739">AKS</span><span class="sxs-lookup"><span data-stu-id="32b2a-739">AKS</span></span>

* <span data-ttu-id="32b2a-740">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-740">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="32b2a-741">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-741">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="32b2a-742">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-742">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="32b2a-743">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-743">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="32b2a-744">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-744">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-745">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-745">AppService</span></span>

* <span data-ttu-id="32b2a-746">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-746">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="32b2a-747">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-747">June 5, 2018</span></span>

<span data-ttu-id="32b2a-748">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="32b2a-748">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-749">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-749">Interactive</span></span>

* <span data-ttu-id="32b2a-750">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-750">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="32b2a-751">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-751">June 5, 2018</span></span>

<span data-ttu-id="32b2a-752">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="32b2a-752">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-753">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-753">Core</span></span>

* <span data-ttu-id="32b2a-754">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-754">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="32b2a-755">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="32b2a-755">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-756">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-756">ACR</span></span>

* <span data-ttu-id="32b2a-757">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-757">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="32b2a-758">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-758">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="32b2a-759">AKS</span><span class="sxs-lookup"><span data-stu-id="32b2a-759">AKS</span></span>

* <span data-ttu-id="32b2a-760">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-760">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-761">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-761">Batch</span></span>

* <span data-ttu-id="32b2a-762">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="32b2a-762">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-763">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-763">IOT</span></span>

* <span data-ttu-id="32b2a-764">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-764">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-765">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-765">Network</span></span>

* <span data-ttu-id="32b2a-766">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-766">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="32b2a-767">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="32b2a-767">Policy Insights</span></span>

* <span data-ttu-id="32b2a-768">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-768">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="32b2a-769">ARM</span><span class="sxs-lookup"><span data-stu-id="32b2a-769">ARM</span></span>

* <span data-ttu-id="32b2a-770">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-770">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-771">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-771">SQL</span></span>

* <span data-ttu-id="32b2a-772">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-772">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="32b2a-773">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-773">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="32b2a-774">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-774">Storage</span></span>

* <span data-ttu-id="32b2a-775">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="32b2a-775">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-776">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-776">VM</span></span>

* <span data-ttu-id="32b2a-777">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-777">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="32b2a-778">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-778">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="32b2a-779">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-779">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="32b2a-780">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-780">May 22, 2018</span></span>

<span data-ttu-id="32b2a-781">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="32b2a-781">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-782">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-782">Core</span></span>

* <span data-ttu-id="32b2a-783">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-783">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-784">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-784">ACS</span></span>

* <span data-ttu-id="32b2a-785">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-785">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="32b2a-786">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-786">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-787">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-787">AppService</span></span>

* <span data-ttu-id="32b2a-788">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="32b2a-788">Improved generic update commands</span></span>
* <span data-ttu-id="32b2a-789">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-789">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-790">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-790">Container</span></span>

* <span data-ttu-id="32b2a-791">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-791">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="32b2a-792">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-792">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-793">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-793">Extension</span></span>

* <span data-ttu-id="32b2a-794">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-794">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-795">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-795">Interactive</span></span>

* <span data-ttu-id="32b2a-796">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-796">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="32b2a-797">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="32b2a-797">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-798">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-798">KeyVault</span></span>

* <span data-ttu-id="32b2a-799">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="32b2a-799">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-800">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-800">Network</span></span>

* <span data-ttu-id="32b2a-801">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="32b2a-801">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="32b2a-802">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="32b2a-802">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-803">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-803">SQL</span></span>

* <span data-ttu-id="32b2a-804">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="32b2a-804">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="32b2a-805">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-805">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="32b2a-806">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-806">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="32b2a-807">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="32b2a-807">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="32b2a-808">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-808">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="32b2a-809">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-809">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="32b2a-810">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="32b2a-810">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="32b2a-811">`edition`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-811">`edition`.</span></span> <span data-ttu-id="32b2a-812">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="32b2a-812">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="32b2a-813">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-813">`elasticPoolName`.</span></span> <span data-ttu-id="32b2a-814">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="32b2a-814">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="32b2a-815">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-815">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="32b2a-816">`edition`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-816">`edition`.</span></span> <span data-ttu-id="32b2a-817">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-817">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="32b2a-818">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-818">`dtu`.</span></span> <span data-ttu-id="32b2a-819">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-819">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="32b2a-820">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-820">`databaseDtuMin`.</span></span> <span data-ttu-id="32b2a-821">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-821">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="32b2a-822">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-822">`databaseDtuMax`.</span></span> <span data-ttu-id="32b2a-823">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-823">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="32b2a-824">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-824">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="32b2a-825">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-825">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-826">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-826">Storage</span></span>

* <span data-ttu-id="32b2a-827">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-827">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="32b2a-828">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-828">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-829">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-829">VM</span></span>

* <span data-ttu-id="32b2a-830">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-830">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="32b2a-831">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-831">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="32b2a-832">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-832">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="32b2a-833">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-833">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="32b2a-834">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-834">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="32b2a-835">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-835">May 7, 2018</span></span>

<span data-ttu-id="32b2a-836">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="32b2a-836">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-837">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-837">Core</span></span>

* <span data-ttu-id="32b2a-838">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="32b2a-838">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="32b2a-839">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-839">Added limited support for positional arguments</span></span>
* <span data-ttu-id="32b2a-840">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-840">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="32b2a-841">#5591</span><span class="sxs-lookup"><span data-stu-id="32b2a-841">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="32b2a-842">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-842">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="32b2a-843">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="32b2a-843">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="32b2a-844">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="32b2a-844">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="32b2a-845">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="32b2a-845">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="32b2a-846">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-846">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-847">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-847">ACR</span></span>

* <span data-ttu-id="32b2a-848">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-848">Added ACR Build commands</span></span>
* <span data-ttu-id="32b2a-849">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-849">Improved resource not found error messages</span></span>
* <span data-ttu-id="32b2a-850">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="32b2a-850">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="32b2a-851">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-851">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="32b2a-852">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-852">Improved repository commands error messages</span></span>
* <span data-ttu-id="32b2a-853">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-853">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-854">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-854">ACS</span></span>

* <span data-ttu-id="32b2a-855">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-855">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="32b2a-856">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-856">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="32b2a-857">AMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-857">AMS</span></span>

* <span data-ttu-id="32b2a-858">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="32b2a-858">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-859">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-859">Appservice</span></span>

* <span data-ttu-id="32b2a-860">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="32b2a-860">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="32b2a-861">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-861">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="32b2a-862">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-862">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="32b2a-863">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-863">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="32b2a-864">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-864">Batch AI</span></span>

* <span data-ttu-id="32b2a-865">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-865">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="32b2a-866">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="32b2a-866">Cognitive Services</span></span>

* <span data-ttu-id="32b2a-867">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="32b2a-867">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-868">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-868">Consumption</span></span>

* <span data-ttu-id="32b2a-869">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-869">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-870">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-870">Container</span></span>

* <span data-ttu-id="32b2a-871">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="32b2a-871">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="32b2a-872">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="32b2a-872">Cosmos DB</span></span>

* <span data-ttu-id="32b2a-873">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="32b2a-873">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="32b2a-874">DMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-874">DMS</span></span>

* <span data-ttu-id="32b2a-875">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-875">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-876">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-876">Extension</span></span>

* <span data-ttu-id="32b2a-877">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-877">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-878">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-878">Interactive</span></span>

* <span data-ttu-id="32b2a-879">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="32b2a-879">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="32b2a-880">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="32b2a-880">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="32b2a-881">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-881">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="32b2a-882">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-882">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="32b2a-883">Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-883">Lab</span></span>

* <span data-ttu-id="32b2a-884">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-884">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-885">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-885">Network</span></span>

* <span data-ttu-id="32b2a-886">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="32b2a-886">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="32b2a-887">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-887">Profile</span></span>

* <span data-ttu-id="32b2a-888">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-888">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="32b2a-889">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-889">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="32b2a-890">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-890">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="32b2a-891">Redis</span><span class="sxs-lookup"><span data-stu-id="32b2a-891">Redis</span></span>

* <span data-ttu-id="32b2a-892">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-892">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="32b2a-893">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-893">Deprecated `redis list-all`.</span></span> <span data-ttu-id="32b2a-894">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-894">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="32b2a-895">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-895">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="32b2a-896">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-896">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-897">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-897">Role</span></span>

* <span data-ttu-id="32b2a-898">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-898">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-899">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-899">Storage</span></span>

* <span data-ttu-id="32b2a-900">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-900">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="32b2a-901">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="32b2a-901">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="32b2a-902">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="32b2a-902">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="32b2a-903">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="32b2a-903">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="32b2a-904">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-904">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-905">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-905">VM</span></span>

* <span data-ttu-id="32b2a-906">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-906">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="32b2a-907">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-907">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="32b2a-908">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="32b2a-908">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="32b2a-909">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-909">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="32b2a-910">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="32b2a-910">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="32b2a-911">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-911">Added write accelerator support</span></span>
* <span data-ttu-id="32b2a-912">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-912">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="32b2a-913">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="32b2a-913">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="32b2a-914">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="32b2a-914">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="32b2a-915">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-915">April 10, 2018</span></span>

<span data-ttu-id="32b2a-916">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="32b2a-916">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-917">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-917">ACR</span></span>

* <span data-ttu-id="32b2a-918">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="32b2a-918">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-919">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-919">ACS</span></span>

* <span data-ttu-id="32b2a-920">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-920">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-921">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-921">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="32b2a-923">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-923">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="32b2a-924">Batch AI</span><span class="sxs-lookup"><span data-stu-id="32b2a-924">BatchAI</span></span>

* <span data-ttu-id="32b2a-925">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-925">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="32b2a-926">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="32b2a-926">Job level mounting</span></span>
  - <span data-ttu-id="32b2a-927">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="32b2a-927">Environment variables with secret values</span></span>
  - <span data-ttu-id="32b2a-928">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="32b2a-928">Performance counters settings</span></span>
  - <span data-ttu-id="32b2a-929">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="32b2a-929">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="32b2a-930">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="32b2a-930">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="32b2a-931">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="32b2a-931">Usage and limits reporting</span></span>
  - <span data-ttu-id="32b2a-932">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="32b2a-932">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="32b2a-933">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="32b2a-933">Support for custom images</span></span>
  - <span data-ttu-id="32b2a-934">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-934">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="32b2a-935">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="32b2a-935">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="32b2a-936">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-936">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="32b2a-937">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="32b2a-937">National clouds are supported</span></span>
* <span data-ttu-id="32b2a-938">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-938">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="32b2a-939">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="32b2a-939">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="32b2a-940">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-940">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="32b2a-941">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="32b2a-941">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="32b2a-942">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="32b2a-942">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="32b2a-943">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="32b2a-943">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="32b2a-944">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="32b2a-944">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="32b2a-945">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-945">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="32b2a-946">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="32b2a-946">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="32b2a-947">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-947">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="32b2a-948">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="32b2a-948">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="32b2a-949">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-949">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="32b2a-950">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="32b2a-950">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="32b2a-951">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="32b2a-951">Billing</span></span>

* <span data-ttu-id="32b2a-952">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-952">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-953">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-953">Consumption</span></span>

* <span data-ttu-id="32b2a-954">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-954">Added `marketplace` commands</span></span>
* <span data-ttu-id="32b2a-955">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-955">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="32b2a-956">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-956">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="32b2a-957">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-957">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="32b2a-958">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-958">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="32b2a-959">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-959">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-960">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-960">Container</span></span>

* <span data-ttu-id="32b2a-961">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-961">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="32b2a-962">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-962">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-963">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-963">Extension</span></span>

* <span data-ttu-id="32b2a-964">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-964">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-965">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-965">Interactive</span></span>

* <span data-ttu-id="32b2a-966">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="32b2a-966">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="32b2a-967">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-967">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="32b2a-968">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-968">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-969">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-969">Network</span></span>

* <span data-ttu-id="32b2a-970">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-970">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="32b2a-971">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-971">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="32b2a-972">#4910</span><span class="sxs-lookup"><span data-stu-id="32b2a-972">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="32b2a-973">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-973">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="32b2a-974">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-974">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="32b2a-975">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-975">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="32b2a-976">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-976">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="32b2a-977">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-977">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-978">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-978">Profile</span></span>

* <span data-ttu-id="32b2a-979">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-979">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="32b2a-980">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-980">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-981">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-981">RDBMS</span></span>

* <span data-ttu-id="32b2a-982">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-982">Added `georestore` command</span></span>
* <span data-ttu-id="32b2a-983">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-983">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-984">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-984">Resource</span></span>

* <span data-ttu-id="32b2a-985">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-985">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="32b2a-986">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-986">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-987">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-987">SQL</span></span>

* <span data-ttu-id="32b2a-988">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-988">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-989">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-989">Storage</span></span>

* <span data-ttu-id="32b2a-990">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-990">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-991">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-991">VM</span></span>

* <span data-ttu-id="32b2a-992">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-992">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="32b2a-993">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-993">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="32b2a-995">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-995">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="32b2a-996">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="32b2a-996">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="32b2a-997">#5718</span><span class="sxs-lookup"><span data-stu-id="32b2a-997">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="32b2a-998">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="32b2a-998">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="32b2a-999">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-999">March 27, 2018</span></span>

<span data-ttu-id="32b2a-1000">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="32b2a-1000">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1001">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1001">Core</span></span>

* <span data-ttu-id="32b2a-1002">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="32b2a-1002">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1003">ACS</span></span>

* <span data-ttu-id="32b2a-1004">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="32b2a-1004">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1005">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1005">Appservice</span></span>

* <span data-ttu-id="32b2a-1006">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1006">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="32b2a-1007">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1007">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="32b2a-1008">Backup</span><span class="sxs-lookup"><span data-stu-id="32b2a-1008">Backup</span></span>

* <span data-ttu-id="32b2a-1009">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1009">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="32b2a-1010">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1010">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="32b2a-1011">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1011">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="32b2a-1012">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1012">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1013">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1013">Container</span></span>

* <span data-ttu-id="32b2a-1014">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1014">Added `container exec` command.</span></span> <span data-ttu-id="32b2a-1015">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="32b2a-1015">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="32b2a-1016">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="32b2a-1016">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-1017">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-1017">Extension</span></span>

* <span data-ttu-id="32b2a-1018">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="32b2a-1018">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="32b2a-1019">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1019">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="32b2a-1020">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1020">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1021">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-1021">Interactive</span></span>

* <span data-ttu-id="32b2a-1022">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1022">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="32b2a-1023">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1023">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="32b2a-1024">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1024">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="32b2a-1025">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1025">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="32b2a-1026">Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1026">Lab</span></span>

* <span data-ttu-id="32b2a-1027">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1027">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1028">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1028">Monitor</span></span>

* <span data-ttu-id="32b2a-1029">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1029">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="32b2a-1030">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="32b2a-1030">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="32b2a-1031">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1031">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1032">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1032">Network</span></span>

* <span data-ttu-id="32b2a-1033">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1033">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1034">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1034">Profile</span></span>

* <span data-ttu-id="32b2a-1035">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1035">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-1036">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1036">RDBMS</span></span>

* <span data-ttu-id="32b2a-1037">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1037">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1038">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1038">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="32b2a-1040">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1040">Role</span></span>

* <span data-ttu-id="32b2a-1041">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1041">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="32b2a-1042">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1042">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="32b2a-1043">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1043">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="32b2a-1044">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1044">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="32b2a-1045">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1045">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1046">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1046">Storage</span></span>

* <span data-ttu-id="32b2a-1047">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1047">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="32b2a-1048">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1048">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1049">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1049">VM</span></span>

* <span data-ttu-id="32b2a-1050">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1050">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="32b2a-1051">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1051">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="32b2a-1052">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1052">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="32b2a-1053">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1053">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="32b2a-1054">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-1054">March 13, 2018</span></span>

<span data-ttu-id="32b2a-1055">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="32b2a-1055">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-1056">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1056">ACR</span></span>

* <span data-ttu-id="32b2a-1057">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1057">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="32b2a-1058">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1058">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="32b2a-1059">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1059">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1060">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1060">ACS</span></span>

* <span data-ttu-id="32b2a-1061">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1061">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="32b2a-1062">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1062">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="32b2a-1063">Advisor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1063">Advisor</span></span>

* <span data-ttu-id="32b2a-1064">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1064">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="32b2a-1065">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1065">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="32b2a-1066">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1066">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="32b2a-1067">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1067">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="32b2a-1068">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1068">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1069">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1069">Appservice</span></span>

* <span data-ttu-id="32b2a-1070">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1070">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="32b2a-1071">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1071">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="32b2a-1072">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="32b2a-1072">Eventhubs</span></span>

* <span data-ttu-id="32b2a-1073">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1073">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-1074">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-1074">Extension</span></span>

* <span data-ttu-id="32b2a-1075">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="32b2a-1075">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1076">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-1076">Interactive</span></span>

* <span data-ttu-id="32b2a-1077">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1077">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="32b2a-1078">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1078">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="32b2a-1079">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1079">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="32b2a-1080">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1080">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1081">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1081">Monitor</span></span>

* <span data-ttu-id="32b2a-1082">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1082">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="32b2a-1083">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1083">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="32b2a-1084">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1084">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="32b2a-1085">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1085">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1086">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1086">Network</span></span>

* <span data-ttu-id="32b2a-1087">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1087">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="32b2a-1088">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1088">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="32b2a-1089">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1089">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="32b2a-1090">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1090">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1091">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1091">Profile</span></span>

* <span data-ttu-id="32b2a-1092">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1092">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="32b2a-1093">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1093">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-1094">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1094">RDBMS</span></span>

* <span data-ttu-id="32b2a-1095">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1095">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="32b2a-1096">Service Bus</span><span class="sxs-lookup"><span data-stu-id="32b2a-1096">Service Bus</span></span>

* <span data-ttu-id="32b2a-1097">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1097">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1098">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1098">Storage</span></span>

* <span data-ttu-id="32b2a-1099">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1099">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="32b2a-1100">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="32b2a-1100">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1101">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1101">VM</span></span>

* <span data-ttu-id="32b2a-1102">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1102">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="32b2a-1103">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1103">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="32b2a-1104">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1104">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="32b2a-1105">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1105">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="32b2a-1106">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-1106">February 27, 2018</span></span>

<span data-ttu-id="32b2a-1107">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="32b2a-1107">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1108">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1108">Core</span></span>

* <span data-ttu-id="32b2a-1109">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="32b2a-1109">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="32b2a-1110">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1110">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="32b2a-1111">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1111">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1112">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1112">ACS</span></span>

* <span data-ttu-id="32b2a-1113">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1113">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="32b2a-1114">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="32b2a-1114">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="32b2a-1115">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1115">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="32b2a-1116">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1116">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1117">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1117">Appservice</span></span>

* <span data-ttu-id="32b2a-1118">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1118">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="32b2a-1119">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1119">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="32b2a-1120">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="32b2a-1120">Cognitive Services</span></span>

* <span data-ttu-id="32b2a-1121">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1121">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-1122">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1122">Consumption</span></span>

* <span data-ttu-id="32b2a-1123">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1123">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="32b2a-1124">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1124">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1125">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1125">Container</span></span>

* <span data-ttu-id="32b2a-1126">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="32b2a-1126">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1127">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1127">Network</span></span>

* <span data-ttu-id="32b2a-1128">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1128">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1129">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1129">Resource</span></span>

* <span data-ttu-id="32b2a-1130">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="32b2a-1130">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1131">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1131">Role</span></span>

* <span data-ttu-id="32b2a-1132">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1132">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1133">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1133">SQL</span></span>

* <span data-ttu-id="32b2a-1134">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1134">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1135">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1135">Storage</span></span>

* <span data-ttu-id="32b2a-1136">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1136">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1137">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1137">VM</span></span>

* <span data-ttu-id="32b2a-1138">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1138">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="32b2a-1139">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-1139">February 13, 2018</span></span>

<span data-ttu-id="32b2a-1140">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="32b2a-1140">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1141">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1141">Core</span></span>

* <span data-ttu-id="32b2a-1142">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1142">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1143">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1143">ACS</span></span>

* <span data-ttu-id="32b2a-1144">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1144">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="32b2a-1145">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1145">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="32b2a-1146">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1146">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="32b2a-1147">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1147">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="32b2a-1148">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1148">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="32b2a-1149">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1149">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="32b2a-1150">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="32b2a-1150">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="32b2a-1151">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="32b2a-1151">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1152">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1152">Appservice</span></span>

* <span data-ttu-id="32b2a-1153">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1153">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="32b2a-1154">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1154">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="32b2a-1155">CDN</span><span class="sxs-lookup"><span data-stu-id="32b2a-1155">CDN</span></span>

* <span data-ttu-id="32b2a-1156">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1156">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1157">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1157">Container</span></span>

* <span data-ttu-id="32b2a-1158">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1158">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="32b2a-1159">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1159">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-1160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-1160">CosmosDB</span></span>

* <span data-ttu-id="32b2a-1161">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1161">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-1162">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-1162">Extension</span></span>

* <span data-ttu-id="32b2a-1163">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1163">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="32b2a-1164">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1164">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="32b2a-1165">Feedback</span><span class="sxs-lookup"><span data-stu-id="32b2a-1165">Feedback</span></span>

* <span data-ttu-id="32b2a-1166">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1166">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1167">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-1167">Interactive</span></span>

* <span data-ttu-id="32b2a-1168">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1168">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="32b2a-1169">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1169">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-1170">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-1170">IoT</span></span>

* <span data-ttu-id="32b2a-1171">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1171">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="32b2a-1172">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1172">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="32b2a-1173">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1173">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="32b2a-1174">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1174">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1175">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1175">Monitor</span></span>

* <span data-ttu-id="32b2a-1176">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1176">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1177">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1177">Network</span></span>

* <span data-ttu-id="32b2a-1178">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1178">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="32b2a-1179">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1179">Profile</span></span>

* <span data-ttu-id="32b2a-1180">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1180">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1181">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1181">Resource</span></span>

* <span data-ttu-id="32b2a-1182">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1182">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1183">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1183">Role</span></span>

* <span data-ttu-id="32b2a-1184">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1184">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1185">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1185">SQL</span></span>

* <span data-ttu-id="32b2a-1186">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1186">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="32b2a-1187">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1187">Added `sql db rename`</span></span>
* <span data-ttu-id="32b2a-1188">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1188">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1189">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1189">Storage</span></span>

* <span data-ttu-id="32b2a-1190">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1190">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1191">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1191">VM</span></span>

* <span data-ttu-id="32b2a-1192">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1192">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="32b2a-1193">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1193">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="32b2a-1194">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1194">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="32b2a-1195">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-1195">January 31, 2018</span></span>

<span data-ttu-id="32b2a-1196">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="32b2a-1196">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1197">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1197">Core</span></span>

* <span data-ttu-id="32b2a-1198">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1198">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="32b2a-1199">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1199">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="32b2a-1200">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1200">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="32b2a-1201">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1201">Use `--verbose` to see</span></span>
* <span data-ttu-id="32b2a-1202">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1202">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1203">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1203">ACS</span></span>

* <span data-ttu-id="32b2a-1204">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1204">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="32b2a-1205">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1205">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1206">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1206">Appservice</span></span>

* <span data-ttu-id="32b2a-1207">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1207">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="32b2a-1208">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1208">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="32b2a-1209">CDN</span><span class="sxs-lookup"><span data-stu-id="32b2a-1209">CDN</span></span>

* <span data-ttu-id="32b2a-1210">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1210">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-1211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-1211">CosmosDB</span></span>

* <span data-ttu-id="32b2a-1212">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1212">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1213">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-1213">Interactive</span></span>

* <span data-ttu-id="32b2a-1214">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1214">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1215">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1215">Network</span></span>

* <span data-ttu-id="32b2a-1216">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1216">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="32b2a-1217">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="32b2a-1217">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="32b2a-1218">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1218">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="32b2a-1219">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1219">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="32b2a-1220">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1220">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="32b2a-1221">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1221">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="32b2a-1222">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1222">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="32b2a-1223">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1223">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="32b2a-1224">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1224">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="32b2a-1225">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1225">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1226">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1226">Profile</span></span>

* <span data-ttu-id="32b2a-1227">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1227">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1228">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1228">Resource</span></span>

* <span data-ttu-id="32b2a-1229">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1229">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1230">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1230">Storage</span></span>

* <span data-ttu-id="32b2a-1231">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1231">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="32b2a-1232">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1232">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="32b2a-1233">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1233">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="32b2a-1234">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1234">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="32b2a-1235">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1235">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1236">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1236">VM</span></span>

* <span data-ttu-id="32b2a-1237">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1237">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="32b2a-1238">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="32b2a-1238">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="32b2a-1239">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1239">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="32b2a-1240">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1240">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="32b2a-1241">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="32b2a-1241">January 17, 2018</span></span>

<span data-ttu-id="32b2a-1242">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="32b2a-1242">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-1243">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1243">ACR</span></span>

* <span data-ttu-id="32b2a-1244">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1244">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="32b2a-1245">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1245">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1246">ACS</span></span>

* <span data-ttu-id="32b2a-1247">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1247">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="32b2a-1248">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1248">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1249">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1249">Appservice</span></span>

* <span data-ttu-id="32b2a-1250">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="32b2a-1250">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="32b2a-1251">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1251">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="32b2a-1252">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1252">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="32b2a-1253">Backup</span><span class="sxs-lookup"><span data-stu-id="32b2a-1253">Backup</span></span>

* <span data-ttu-id="32b2a-1254">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1254">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="32b2a-1255">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1255">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="32b2a-1256">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1256">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="32b2a-1257">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1257">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="32b2a-1258">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1258">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-1259">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-1259">Batch</span></span>

* <span data-ttu-id="32b2a-1260">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1260">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="32b2a-1261">Cloud</span><span class="sxs-lookup"><span data-stu-id="32b2a-1261">Cloud</span></span>

* <span data-ttu-id="32b2a-1262">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1262">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-1263">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1263">Consumption</span></span>

* <span data-ttu-id="32b2a-1264">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1264">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="32b2a-1265">Event Grid</span><span class="sxs-lookup"><span data-stu-id="32b2a-1265">Event Grid</span></span>

* <span data-ttu-id="32b2a-1266">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1266">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="32b2a-1267">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1267">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="32b2a-1268">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1268">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="32b2a-1269">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1269">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="32b2a-1270">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1270">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="32b2a-1271">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1271">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="32b2a-1272">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1272">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="32b2a-1273">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1273">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1274">Interactive</span><span class="sxs-lookup"><span data-stu-id="32b2a-1274">Interactive</span></span>

* <span data-ttu-id="32b2a-1275">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1275">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="32b2a-1276">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1276">Fixed errors on startup</span></span>
* <span data-ttu-id="32b2a-1277">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1277">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-1278">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-1278">IoT</span></span>

* <span data-ttu-id="32b2a-1279">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1279">Added support for device provisioning service</span></span>
* <span data-ttu-id="32b2a-1280">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1280">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="32b2a-1281">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-1281">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1282">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1282">Monitor</span></span>

* <span data-ttu-id="32b2a-1283">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1283">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="32b2a-1284">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1284">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="32b2a-1285">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1285">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1286">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1286">Network</span></span>

* <span data-ttu-id="32b2a-1287">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1287">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="32b2a-1288">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1288">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1289">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1289">Profile</span></span>

* <span data-ttu-id="32b2a-1290">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1290">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1291">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1291">Role</span></span>

* <span data-ttu-id="32b2a-1292">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1292">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="32b2a-1293">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="32b2a-1293">Service Fabric</span></span>

* <span data-ttu-id="32b2a-1294">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1294">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="32b2a-1295">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1295">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1296">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1296">VM</span></span>

* <span data-ttu-id="32b2a-1297">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1297">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="32b2a-1298">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1298">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="32b2a-1299">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="32b2a-1299">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="32b2a-1300">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1300">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="32b2a-1301">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1301">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="32b2a-1302">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1302">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="32b2a-1303">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1303">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="32b2a-1304">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1304">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="32b2a-1305">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1305">December 19, 2017</span></span>

<span data-ttu-id="32b2a-1306">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="32b2a-1306">Version 2.0.23</span></span>

* <span data-ttu-id="32b2a-1307">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1307">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1308">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1308">Container</span></span>

* <span data-ttu-id="32b2a-1309">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1309">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1310">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1310">Network</span></span>

* <span data-ttu-id="32b2a-1311">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1311">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="32b2a-1312">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1312">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1313">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1313">Storage</span></span>

* <span data-ttu-id="32b2a-1314">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1314">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1315">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1315">VM</span></span>

* <span data-ttu-id="32b2a-1316">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1316">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="32b2a-1317">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1317">December 5, 2017</span></span>

<span data-ttu-id="32b2a-1318">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="32b2a-1318">Version 2.0.22</span></span>

* <span data-ttu-id="32b2a-1319">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1319">Removed `az component` commands.</span></span> <span data-ttu-id="32b2a-1320">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1320">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1321">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1321">Core</span></span>
* <span data-ttu-id="32b2a-1322">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1322">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="32b2a-1323">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1323">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1324">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1324">ACS</span></span>

* <span data-ttu-id="32b2a-1325">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1325">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="32b2a-1326">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1326">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="32b2a-1327">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="32b2a-1327">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="32b2a-1328">Advisor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1328">Advisor</span></span>

* <span data-ttu-id="32b2a-1329">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1329">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1330">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1330">Appservice</span></span>

* <span data-ttu-id="32b2a-1331">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1331">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="32b2a-1332">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1332">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="32b2a-1333">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1333">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="32b2a-1334">Nutzung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1334">Consumption</span></span>

* <span data-ttu-id="32b2a-1335">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1335">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1336">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1336">Container</span></span>

* <span data-ttu-id="32b2a-1337">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="32b2a-1337">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1338">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1338">Monitor</span></span>

* <span data-ttu-id="32b2a-1339">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1339">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1340">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1340">Resource</span></span>

* <span data-ttu-id="32b2a-1341">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1341">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1342">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1342">Role</span></span>

* <span data-ttu-id="32b2a-1343">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1343">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="32b2a-1344">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1344">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="32b2a-1345">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1345">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1346">SQL</span></span>

* <span data-ttu-id="32b2a-1347">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1347">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="32b2a-1348">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1348">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1349">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1349">VM</span></span>

* <span data-ttu-id="32b2a-1350">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1350">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="32b2a-1351">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1351">November 14, 2017</span></span>

<span data-ttu-id="32b2a-1352">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="32b2a-1352">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-1353">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1353">ACR</span></span>

* <span data-ttu-id="32b2a-1354">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1354">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="32b2a-1355">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1355">ACS</span></span>

* <span data-ttu-id="32b2a-1356">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1356">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="32b2a-1357">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="32b2a-1357">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="32b2a-1358">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1358">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="32b2a-1359">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1359">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="32b2a-1360">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1360">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1361">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1361">Appservice</span></span>

* <span data-ttu-id="32b2a-1362">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1362">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="32b2a-1363">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1363">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="32b2a-1364">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1364">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="32b2a-1365">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1365">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="32b2a-1366">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1366">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="32b2a-1367">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1367">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-1368">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-1368">Batch</span></span>

* <span data-ttu-id="32b2a-1369">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1369">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="32b2a-1370">BatchAI</span><span class="sxs-lookup"><span data-stu-id="32b2a-1370">Batchai</span></span>

* <span data-ttu-id="32b2a-1371">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1371">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="32b2a-1372">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1372">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="32b2a-1373">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1373">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="32b2a-1374">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1374">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="32b2a-1375">Cloud</span><span class="sxs-lookup"><span data-stu-id="32b2a-1375">Cloud</span></span>

* <span data-ttu-id="32b2a-1376">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="32b2a-1376">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1377">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1377">Container</span></span>

* <span data-ttu-id="32b2a-1378">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1378">Added support to open multiple ports</span></span>
* <span data-ttu-id="32b2a-1379">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1379">Added container group restart policy</span></span>
* <span data-ttu-id="32b2a-1380">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1380">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="32b2a-1381">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1381">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="32b2a-1382">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="32b2a-1382">Data Lake Analytics</span></span>

* <span data-ttu-id="32b2a-1383">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1383">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="32b2a-1384">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="32b2a-1384">Data Lake Store</span></span>

* <span data-ttu-id="32b2a-1385">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1385">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-1386">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-1386">Extension</span></span>

* <span data-ttu-id="32b2a-1387">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1387">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="32b2a-1388">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1388">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-1389">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-1389">IoT</span></span>

* <span data-ttu-id="32b2a-1390">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1390">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1391">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1391">Monitor</span></span>

* <span data-ttu-id="32b2a-1392">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1392">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1393">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1393">Network</span></span>

* <span data-ttu-id="32b2a-1394">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1394">Added support for CAA DNS records</span></span>
* <span data-ttu-id="32b2a-1395">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1395">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="32b2a-1396">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1396">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="32b2a-1397">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1397">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="32b2a-1398">Reservations</span><span class="sxs-lookup"><span data-stu-id="32b2a-1398">Reservations</span></span>

* <span data-ttu-id="32b2a-1399">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="32b2a-1399">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1400">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1400">Resource</span></span>

* <span data-ttu-id="32b2a-1401">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1401">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1402">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1402">SQL</span></span>

* <span data-ttu-id="32b2a-1403">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1403">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1404">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1404">Storage</span></span>

* <span data-ttu-id="32b2a-1405">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1405">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="32b2a-1406">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1406">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="32b2a-1407">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1407">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="32b2a-1408">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1408">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="32b2a-1409">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1409">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="32b2a-1410">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1410">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="32b2a-1411">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1411">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1412">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1412">VM</span></span>

* <span data-ttu-id="32b2a-1413">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1413">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="32b2a-1414">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1414">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="32b2a-1415">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="32b2a-1415">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="32b2a-1416">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1416">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="32b2a-1417">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1417">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="32b2a-1418">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1418">October 24, 2017</span></span>

<span data-ttu-id="32b2a-1419">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="32b2a-1419">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1420">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1420">Core</span></span>

* <span data-ttu-id="32b2a-1421">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="32b2a-1421">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1422">ACR</span></span>

* <span data-ttu-id="32b2a-1423">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1423">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="32b2a-1424">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1424">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="32b2a-1425">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1425">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1426">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1426">ACS</span></span>

* <span data-ttu-id="32b2a-1427">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1427">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="32b2a-1428">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1428">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1429">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1429">Appservice</span></span>

* <span data-ttu-id="32b2a-1430">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="32b2a-1430">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="32b2a-1431">Komponente</span><span class="sxs-lookup"><span data-stu-id="32b2a-1431">Component</span></span>

* <span data-ttu-id="32b2a-1432">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1432">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1433">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1433">Monitor</span></span>

* <span data-ttu-id="32b2a-1434">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1434">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1435">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1435">Resource</span></span>

* <span data-ttu-id="32b2a-1436">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1436">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="32b2a-1437">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="32b2a-1437">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1438">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1438">VM</span></span>

* <span data-ttu-id="32b2a-1439">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1439">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="32b2a-1440">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1440">October 9, 2017</span></span>

<span data-ttu-id="32b2a-1441">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="32b2a-1441">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1442">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1442">Core</span></span>

* <span data-ttu-id="32b2a-1443">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1443">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1444">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1444">Appservice</span></span>

* <span data-ttu-id="32b2a-1445">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1445">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-1446">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-1446">Batch</span></span>

* <span data-ttu-id="32b2a-1447">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="32b2a-1447">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="32b2a-1448">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1448">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="32b2a-1449">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1449">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="32b2a-1450">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1450">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="32b2a-1451">BatchAI</span><span class="sxs-lookup"><span data-stu-id="32b2a-1451">Batchai</span></span>

* <span data-ttu-id="32b2a-1452">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1452">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-1453">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-1453">Keyvault</span></span>

* <span data-ttu-id="32b2a-1454">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1454">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="32b2a-1455">(#4448)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1455">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="32b2a-1456">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1456">Network</span></span>

* <span data-ttu-id="32b2a-1457">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1457">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="32b2a-1458">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1458">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1459">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1459">Resource</span></span>

* <span data-ttu-id="32b2a-1460">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1460">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="32b2a-1461">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1461">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="32b2a-1462">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1462">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="32b2a-1463">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1463">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1464">Sql</span><span class="sxs-lookup"><span data-stu-id="32b2a-1464">Sql</span></span>

* <span data-ttu-id="32b2a-1465">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1465">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="32b2a-1466">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1466">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="32b2a-1467">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1467">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1468">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1468">Storage</span></span>

* <span data-ttu-id="32b2a-1469">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1469">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1470">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1470">Vm</span></span>

* <span data-ttu-id="32b2a-1471">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1471">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="32b2a-1472">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1472">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="32b2a-1473">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1473">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="32b2a-1474">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1474">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="32b2a-1475">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1475">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="32b2a-1476">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1476">September 22, 2017</span></span>

<span data-ttu-id="32b2a-1477">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="32b2a-1477">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1478">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1478">Resource</span></span>

* <span data-ttu-id="32b2a-1479">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1479">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="32b2a-1480">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1480">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="32b2a-1481">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1481">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="32b2a-1482">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1482">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1483">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1483">Network</span></span>

* <span data-ttu-id="32b2a-1484">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1484">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="32b2a-1485">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1485">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="32b2a-1486">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1486">Added `asg` application security group commands</span></span>
* <span data-ttu-id="32b2a-1487">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1487">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="32b2a-1488">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1488">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="32b2a-1489">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1489">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="32b2a-1490">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1490">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1491">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1491">Storage</span></span>

* <span data-ttu-id="32b2a-1492">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1492">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="32b2a-1493">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="32b2a-1493">Eventgrid</span></span>

* <span data-ttu-id="32b2a-1494">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1494">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1495">SQL</span></span>

* <span data-ttu-id="32b2a-1496">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1496">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="32b2a-1497">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1497">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="32b2a-1498">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1498">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-1499">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-1499">Keyvault</span></span>

* <span data-ttu-id="32b2a-1500">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1500">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1501">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1501">VM</span></span>

* <span data-ttu-id="32b2a-1502">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1502">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="32b2a-1503">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1503">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="32b2a-1504">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1504">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="32b2a-1505">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1505">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="32b2a-1506">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1506">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="32b2a-1507">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1507">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1508">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1508">ACS</span></span>

* <span data-ttu-id="32b2a-1509">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1509">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1510">Appservice</span></span>

* <span data-ttu-id="32b2a-1511">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1511">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="32b2a-1512">Backup</span><span class="sxs-lookup"><span data-stu-id="32b2a-1512">Backup</span></span>

* <span data-ttu-id="32b2a-1513">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="32b2a-1513">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="32b2a-1514">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1514">September 11, 2017</span></span>

<span data-ttu-id="32b2a-1515">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="32b2a-1515">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="32b2a-1516">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1516">Core</span></span>

* <span data-ttu-id="32b2a-1517">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1517">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="32b2a-1518">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1518">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1519">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1519">Acs</span></span>

* <span data-ttu-id="32b2a-1520">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1520">Added `acs list-locations` command</span></span>
* <span data-ttu-id="32b2a-1521">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1521">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1522">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1522">Appservice</span></span>

* <span data-ttu-id="32b2a-1523">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="32b2a-1523">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="32b2a-1524">CDN</span><span class="sxs-lookup"><span data-stu-id="32b2a-1524">CDN</span></span>

* <span data-ttu-id="32b2a-1525">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1525">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="32b2a-1526">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="32b2a-1526">Extension</span></span>

* <span data-ttu-id="32b2a-1527">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1527">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-1528">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-1528">Keyvault</span></span>

* <span data-ttu-id="32b2a-1529">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="32b2a-1529">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1530">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1530">Network</span></span>

* <span data-ttu-id="32b2a-1531">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1531">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="32b2a-1532">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1532">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="32b2a-1533">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1533">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="32b2a-1534">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1534">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="32b2a-1535">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1535">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1536">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1536">Resource</span></span>

* <span data-ttu-id="32b2a-1537">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1537">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="32b2a-1538">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1538">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="32b2a-1539">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1539">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="32b2a-1540">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1540">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1541">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1541">SQL</span></span>

* <span data-ttu-id="32b2a-1542">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1542">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1543">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1543">VM</span></span>

* <span data-ttu-id="32b2a-1544">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1544">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="32b2a-1545">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1545">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="32b2a-1546">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1546">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="32b2a-1547">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1547">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="32b2a-1548">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1548">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="32b2a-1549">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1549">August 31, 2017</span></span>

<span data-ttu-id="32b2a-1550">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="32b2a-1550">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-1551">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-1551">Keyvault</span></span>

* <span data-ttu-id="32b2a-1552">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1552">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="32b2a-1553">Sf</span><span class="sxs-lookup"><span data-stu-id="32b2a-1553">Sf</span></span>

* <span data-ttu-id="32b2a-1554">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1554">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1555">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1555">Storage</span></span>

* <span data-ttu-id="32b2a-1556">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1556">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="32b2a-1557">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="32b2a-1557">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="32b2a-1558">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1558">August 28, 2017</span></span>

<span data-ttu-id="32b2a-1559">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="32b2a-1559">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="32b2a-1560">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1560">CLI</span></span>

* <span data-ttu-id="32b2a-1561">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1561">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1562">ACS</span></span>

* <span data-ttu-id="32b2a-1563">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1563">Corrected preview regions</span></span>
* <span data-ttu-id="32b2a-1564">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1564">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="32b2a-1565">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1565">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1566">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1566">Appservice</span></span>

* <span data-ttu-id="32b2a-1567">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1567">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="32b2a-1568">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1568">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="32b2a-1569">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1569">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="32b2a-1570">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1570">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="32b2a-1571">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1571">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-1572">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-1572">IoT</span></span>

* <span data-ttu-id="32b2a-1573">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="32b2a-1573">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1574">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1574">Network</span></span>

* <span data-ttu-id="32b2a-1575">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1575">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="32b2a-1576">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1576">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="32b2a-1577">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1577">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="32b2a-1578">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1578">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="32b2a-1579">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1579">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1580">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1580">Profile</span></span>

* <span data-ttu-id="32b2a-1581">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1581">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="32b2a-1582">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="32b2a-1582">Service Fabric</span></span>

* <span data-ttu-id="32b2a-1583">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="32b2a-1583">Preview release</span></span>
* <span data-ttu-id="32b2a-1584">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1584">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="32b2a-1585">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1585">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="32b2a-1586">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1586">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1587">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1587">Storage</span></span>

* <span data-ttu-id="32b2a-1588">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1588">Enabled setting blob tier</span></span>
* <span data-ttu-id="32b2a-1589">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1589">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="32b2a-1590">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1590">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="32b2a-1591">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1591">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="32b2a-1592">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1592">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="32b2a-1593">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1593">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1594">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1594">VM</span></span>

* <span data-ttu-id="32b2a-1595">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1595">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="32b2a-1596">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1596">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="32b2a-1597">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1597">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="32b2a-1598">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1598">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="32b2a-1599">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1599">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="32b2a-1600">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1600">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="32b2a-1601">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1601">August 15, 2017</span></span>

<span data-ttu-id="32b2a-1602">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="32b2a-1602">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1603">ACS</span></span>

* <span data-ttu-id="32b2a-1604">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1604">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1605">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1605">Appservice</span></span>

* <span data-ttu-id="32b2a-1606">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1606">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="32b2a-1607">Event Grid</span><span class="sxs-lookup"><span data-stu-id="32b2a-1607">Event Grid</span></span>

* <span data-ttu-id="32b2a-1608">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1608">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="32b2a-1609">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1609">August 11, 2017</span></span>

<span data-ttu-id="32b2a-1610">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="32b2a-1610">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1611">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1611">ACS</span></span>

* <span data-ttu-id="32b2a-1612">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1612">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-1613">Batch</span></span>

* <span data-ttu-id="32b2a-1614">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1614">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="32b2a-1615">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1615">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="32b2a-1616">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1616">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="32b2a-1617">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1617">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="32b2a-1618">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="32b2a-1618">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="32b2a-1619">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1619">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="32b2a-1620">Komponente</span><span class="sxs-lookup"><span data-stu-id="32b2a-1620">Component</span></span>

* <span data-ttu-id="32b2a-1621">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1621">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="32b2a-1622">Container</span><span class="sxs-lookup"><span data-stu-id="32b2a-1622">Container</span></span>

* <span data-ttu-id="32b2a-1623">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="32b2a-1623">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="32b2a-1624">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="32b2a-1624">Data Lake Store</span></span>

* <span data-ttu-id="32b2a-1625">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1625">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="32b2a-1626">Event Grid</span><span class="sxs-lookup"><span data-stu-id="32b2a-1626">Event Grid</span></span>

* <span data-ttu-id="32b2a-1627">Erste Version</span><span class="sxs-lookup"><span data-stu-id="32b2a-1627">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1628">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1628">Network</span></span>

* <span data-ttu-id="32b2a-1629">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1629">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="32b2a-1630">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-1630">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="32b2a-1631">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1631">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="32b2a-1632">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1632">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1633">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1633">Profile</span></span>

* <span data-ttu-id="32b2a-1634">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="32b2a-1634">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1635">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1635">Storage</span></span>

* <span data-ttu-id="32b2a-1636">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1636">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1637">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1637">VM</span></span>

* <span data-ttu-id="32b2a-1638">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1638">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="32b2a-1639">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1639">Exposed `list-skus` command</span></span>
* <span data-ttu-id="32b2a-1640">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1640">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="32b2a-1641">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="32b2a-1641">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="32b2a-1642">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1642">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="32b2a-1643">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1643">July 28, 2017</span></span>

<span data-ttu-id="32b2a-1644">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="32b2a-1644">Version 2.0.12</span></span>

* <span data-ttu-id="32b2a-1645">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1645">Added container commands</span></span>
* <span data-ttu-id="32b2a-1646">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1646">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="32b2a-1647">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1647">Core</span></span>

* <span data-ttu-id="32b2a-1648">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1648">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="32b2a-1649">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1649">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="32b2a-1650">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="32b2a-1650">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="32b2a-1651">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1651">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="32b2a-1652">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1652">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="32b2a-1653">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1653">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="32b2a-1654">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1654">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="32b2a-1655">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1655">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="32b2a-1656">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1656">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="32b2a-1657">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1657">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="32b2a-1658">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="32b2a-1658">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="32b2a-1659">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1659">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="32b2a-1660">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1660">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="32b2a-1661">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1661">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="32b2a-1662">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="32b2a-1662">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="32b2a-1663">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1663">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="32b2a-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1664">ACR</span></span>

* <span data-ttu-id="32b2a-1665">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1665">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="32b2a-1666">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1666">Support SKU update for managed registries</span></span>
* <span data-ttu-id="32b2a-1667">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1667">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="32b2a-1668">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1668">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="32b2a-1669">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1669">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="32b2a-1670">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1670">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1671">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1671">ACS</span></span>

* <span data-ttu-id="32b2a-1672">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="32b2a-1672">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1673">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1673">Appservice</span></span>

* <span data-ttu-id="32b2a-1674">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1674">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="32b2a-1675">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="32b2a-1675">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="32b2a-1676">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1676">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="32b2a-1677">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1677">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="32b2a-1678">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1678">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="32b2a-1679">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1679">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="32b2a-1680">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1680">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="32b2a-1681">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1681">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="32b2a-1682">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1682">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="32b2a-1683">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1683">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="32b2a-1684">Batch</span><span class="sxs-lookup"><span data-stu-id="32b2a-1684">Batch</span></span>

* <span data-ttu-id="32b2a-1685">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1685">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="32b2a-1686">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1686">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="32b2a-1687">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1687">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="32b2a-1688">CDN</span><span class="sxs-lookup"><span data-stu-id="32b2a-1688">CDN</span></span>

* <span data-ttu-id="32b2a-1689">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1689">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="32b2a-1690">Cloud</span><span class="sxs-lookup"><span data-stu-id="32b2a-1690">Cloud</span></span>

* <span data-ttu-id="32b2a-1691">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1691">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="32b2a-1692">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="32b2a-1692">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="32b2a-1693">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1693">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="32b2a-1694">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="32b2a-1694">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="32b2a-1695">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1695">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-1696">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-1696">CosmosDB</span></span>

* <span data-ttu-id="32b2a-1697">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1697">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="32b2a-1698">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1698">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="32b2a-1699">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="32b2a-1699">Data Lake Analytics</span></span>

* <span data-ttu-id="32b2a-1700">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1700">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="32b2a-1701">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1701">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="32b2a-1702">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1702">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="32b2a-1703">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="32b2a-1703">Data Lake Store</span></span>

* <span data-ttu-id="32b2a-1704">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1704">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="32b2a-1705">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="32b2a-1705">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="32b2a-1706">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1706">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="32b2a-1707">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1707">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="32b2a-1708">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="32b2a-1708">Interactive</span></span>

* <span data-ttu-id="32b2a-1709">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1709">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="32b2a-1710">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1710">Increased test coverage</span></span>
* <span data-ttu-id="32b2a-1711">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1711">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="32b2a-1712">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1712">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="32b2a-1713">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1713">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="32b2a-1714">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1714">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="32b2a-1715">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1715">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="32b2a-1716">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1716">Added `--progress` flag</span></span>
* <span data-ttu-id="32b2a-1717">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1717">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="32b2a-1718">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1718">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="32b2a-1719">IoT</span><span class="sxs-lookup"><span data-stu-id="32b2a-1719">IoT</span></span>

* <span data-ttu-id="32b2a-1720">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="32b2a-1720">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="32b2a-1721">(3934)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1721">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="32b2a-1722">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1722">Key vault</span></span>

* <span data-ttu-id="32b2a-1723">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1723">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="32b2a-1724">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1724">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="32b2a-1725">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1725">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="32b2a-1726">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1726">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="32b2a-1727">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1727">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="32b2a-1728">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1728">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="32b2a-1729">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1729">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="32b2a-1730">(3307)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1730">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="32b2a-1731">Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1731">Lab</span></span>

* <span data-ttu-id="32b2a-1732">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1732">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="32b2a-1733">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1733">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1734">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1734">Monitor</span></span>

* <span data-ttu-id="32b2a-1735">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1735">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="32b2a-1736">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1736">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="32b2a-1737">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1737">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="32b2a-1738">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1738">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="32b2a-1739">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1739">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="32b2a-1740">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1740">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="32b2a-1741">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1741">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="32b2a-1742">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1742">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="32b2a-1743">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="32b2a-1743">`location` no longer required</span></span>
  * <span data-ttu-id="32b2a-1744">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="32b2a-1744">Add name and ID support for target</span></span>
  * <span data-ttu-id="32b2a-1745">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1745">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="32b2a-1746">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1746">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="32b2a-1747">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1747">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="32b2a-1748">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="32b2a-1748">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="32b2a-1749">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1749">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="32b2a-1750">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1750">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1751">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1751">Network</span></span>

* <span data-ttu-id="32b2a-1752">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1752">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="32b2a-1753">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1753">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="32b2a-1754">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1754">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="32b2a-1755">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1755">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="32b2a-1756">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1756">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="32b2a-1757">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1757">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="32b2a-1758">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1758">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="32b2a-1759">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1759">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="32b2a-1760">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1760">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="32b2a-1761">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1761">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="32b2a-1762">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1762">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="32b2a-1763">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1763">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="32b2a-1764">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1764">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="32b2a-1765">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1765">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="32b2a-1766">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1766">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="32b2a-1767">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1767">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="32b2a-1768">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="32b2a-1768">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="32b2a-1769">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-1769">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="32b2a-1770">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1770">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="32b2a-1771">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1771">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="32b2a-1772">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1772">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="32b2a-1773">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1773">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="32b2a-1774">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1774">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="32b2a-1775">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1775">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="32b2a-1776">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1776">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="32b2a-1777">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1777">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="32b2a-1778">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1778">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1779">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1779">Profile</span></span>

* <span data-ttu-id="32b2a-1780">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="32b2a-1780">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="32b2a-1781">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="32b2a-1781">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="32b2a-1782">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1782">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="32b2a-1783">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1783">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="32b2a-1784">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="32b2a-1784">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="32b2a-1785">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1785">RDBMS</span></span>

* <span data-ttu-id="32b2a-1786">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1786">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="32b2a-1787">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1787">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="32b2a-1788">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1788">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="32b2a-1789">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1789">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1790">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1790">Resource</span></span>

* <span data-ttu-id="32b2a-1791">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1791">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="32b2a-1792">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="32b2a-1792">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="32b2a-1793">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1793">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="32b2a-1794">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1794">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="32b2a-1795">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1795">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="32b2a-1796">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1796">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="32b2a-1797">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1797">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="32b2a-1798">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1798">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1799">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1799">Role</span></span>

* <span data-ttu-id="32b2a-1800">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1800">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="32b2a-1801">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1801">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="32b2a-1802">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="32b2a-1802">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="32b2a-1803">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1803">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="32b2a-1804">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1804">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="32b2a-1805">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="32b2a-1805">Service Fabric</span></span>
* <span data-ttu-id="32b2a-1806">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1806">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="32b2a-1807">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1807">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="32b2a-1808">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1808">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1809">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1809">SQL</span></span>

* <span data-ttu-id="32b2a-1810">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1810">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="32b2a-1811">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1811">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="32b2a-1812">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1812">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1813">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1813">Storage</span></span>

* <span data-ttu-id="32b2a-1814">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1814">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="32b2a-1815">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1815">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="32b2a-1816">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1816">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="32b2a-1817">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1817">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="32b2a-1818">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1818">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="32b2a-1819">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1819">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1820">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1820">VM</span></span>

* <span data-ttu-id="32b2a-1821">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="32b2a-1821">Support configuring nsg</span></span>
* <span data-ttu-id="32b2a-1822">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-1822">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="32b2a-1823">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1823">Support managed service identities</span></span>
* <span data-ttu-id="32b2a-1824">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1824">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="32b2a-1825">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1825">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="32b2a-1826">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1826">May 10, 2017</span></span>

<span data-ttu-id="32b2a-1827">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="32b2a-1827">Version 2.0.6</span></span>

* <span data-ttu-id="32b2a-1828">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1828">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="32b2a-1829">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1829">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="32b2a-1830">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="32b2a-1830">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="32b2a-1831">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1831">Include Cognitive Services module</span></span>
* <span data-ttu-id="32b2a-1832">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1832">Include Service Fabric module</span></span>
* <span data-ttu-id="32b2a-1833">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1833">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="32b2a-1834">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1834">Add support for CDN commands</span></span>
* <span data-ttu-id="32b2a-1835">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1835">Remove Container module</span></span>
* <span data-ttu-id="32b2a-1836">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1836">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="32b2a-1837">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1837">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="32b2a-1838">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1838">Core</span></span>

* <span data-ttu-id="32b2a-1839">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1839">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="32b2a-1840">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1840">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="32b2a-1841">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1841">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="32b2a-1842">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1842">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="32b2a-1843">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1843">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="32b2a-1844">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1844">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="32b2a-1845">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1845">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="32b2a-1846">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1846">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="32b2a-1847">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1847">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="32b2a-1848">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1848">core: Improved performance</span></span>
* <span data-ttu-id="32b2a-1849">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1849">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="32b2a-1850">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1850">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1851">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1851">ACS</span></span>

* <span data-ttu-id="32b2a-1852">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32b2a-1852">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="32b2a-1853">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1853">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="32b2a-1854">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1854">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="32b2a-1855">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1855">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1856">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1856">AppService</span></span>

* <span data-ttu-id="32b2a-1857">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1857">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="32b2a-1858">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1858">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="32b2a-1859">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="32b2a-1859">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="32b2a-1860">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="32b2a-1860">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="32b2a-1861">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1861">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="32b2a-1862">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1862">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="32b2a-1863">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="32b2a-1863">support slot swap with preview</span></span>
* <span data-ttu-id="32b2a-1864">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1864">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="32b2a-1865">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1865">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32b2a-1866">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-1866">CosmosDB</span></span>

* <span data-ttu-id="32b2a-1867">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="32b2a-1867">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="32b2a-1868">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1868">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="32b2a-1869">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1869">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="32b2a-1870">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="32b2a-1870">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="32b2a-1871">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="32b2a-1871">Data Lake Analytics</span></span>

* <span data-ttu-id="32b2a-1872">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="32b2a-1872">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="32b2a-1873">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1873">Add support for new catalog item type: package.</span></span> <span data-ttu-id="32b2a-1874">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1874">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="32b2a-1875">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="32b2a-1875">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="32b2a-1876">Table</span><span class="sxs-lookup"><span data-stu-id="32b2a-1876">Table</span></span>
  * <span data-ttu-id="32b2a-1877">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="32b2a-1877">Table valued function</span></span>
  * <span data-ttu-id="32b2a-1878">Sicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1878">View</span></span>
  * <span data-ttu-id="32b2a-1879">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1879">Table Statistics.</span></span> <span data-ttu-id="32b2a-1880">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1880">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="32b2a-1881">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="32b2a-1881">Data Lake Store</span></span>

* <span data-ttu-id="32b2a-1882">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1882">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="32b2a-1883">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1883">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="32b2a-1884">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="32b2a-1884">missed help for access show.</span></span> <span data-ttu-id="32b2a-1885">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="32b2a-1885">adding it.</span></span> <span data-ttu-id="32b2a-1886">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1886">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="32b2a-1887">Suchen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1887">Find</span></span>

* <span data-ttu-id="32b2a-1888">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="32b2a-1888">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="32b2a-1889">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32b2a-1889">KeyVault</span></span>

* <span data-ttu-id="32b2a-1890">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1890">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="32b2a-1891">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1891">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="32b2a-1892">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="32b2a-1892">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="32b2a-1893">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="32b2a-1893">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="32b2a-1894">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1894">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="32b2a-1895">Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1895">Lab</span></span>

* <span data-ttu-id="32b2a-1896">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="32b2a-1896">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="32b2a-1897">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1897">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="32b2a-1898">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="32b2a-1898">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="32b2a-1899">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="32b2a-1899">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="32b2a-1900">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="32b2a-1900">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="32b2a-1901">Überwachen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1901">Monitor</span></span>

* <span data-ttu-id="32b2a-1902">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1902">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="32b2a-1903">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1903">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="32b2a-1904">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1904">Network</span></span>

* <span data-ttu-id="32b2a-1905">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1905">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="32b2a-1906">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1906">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="32b2a-1907">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="32b2a-1907">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="32b2a-1908">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1908">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="32b2a-1909">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="32b2a-1909">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="32b2a-1910">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="32b2a-1910">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="32b2a-1911">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1911">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="32b2a-1912">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1912">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="32b2a-1913">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1913">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="32b2a-1914">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="32b2a-1914">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="32b2a-1915">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1915">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="32b2a-1916">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1916">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="32b2a-1917">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="32b2a-1917">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="32b2a-1918">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="32b2a-1918">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="32b2a-1919">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="32b2a-1919">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="32b2a-1920">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1920">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="32b2a-1921">Profil</span><span class="sxs-lookup"><span data-stu-id="32b2a-1921">Profile</span></span>

* <span data-ttu-id="32b2a-1922">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1922">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="32b2a-1923">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1923">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="32b2a-1924">Redis</span><span class="sxs-lookup"><span data-stu-id="32b2a-1924">Redis</span></span>

* <span data-ttu-id="32b2a-1925">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1925">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="32b2a-1926">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1926">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="32b2a-1927">Ressource</span><span class="sxs-lookup"><span data-stu-id="32b2a-1927">Resource</span></span>

* <span data-ttu-id="32b2a-1928">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1928">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="32b2a-1929">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1929">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="32b2a-1930">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1930">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="32b2a-1931">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="32b2a-1931">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="32b2a-1932">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1932">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="32b2a-1933">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1933">Add docs for az lock update.</span></span> <span data-ttu-id="32b2a-1934">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1934">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="32b2a-1935">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1935">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="32b2a-1936">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1936">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="32b2a-1937">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="32b2a-1937">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="32b2a-1938">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1938">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="32b2a-1939">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1939">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="32b2a-1940">Rolle</span><span class="sxs-lookup"><span data-stu-id="32b2a-1940">Role</span></span>

* <span data-ttu-id="32b2a-1941">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1941">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="32b2a-1942">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1942">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="32b2a-1943">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1943">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="32b2a-1944">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="32b2a-1944">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="32b2a-1945">SQL</span><span class="sxs-lookup"><span data-stu-id="32b2a-1945">SQL</span></span>

* <span data-ttu-id="32b2a-1946">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1946">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="32b2a-1947">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1947">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="32b2a-1948">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-1948">Storage</span></span>

* <span data-ttu-id="32b2a-1949">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="32b2a-1949">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="32b2a-1950">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="32b2a-1950">Add support for incremental blob copy</span></span>
* <span data-ttu-id="32b2a-1951">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="32b2a-1951">Add support for large block blob upload</span></span>
* <span data-ttu-id="32b2a-1952">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="32b2a-1952">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1953">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1953">VM</span></span>

* <span data-ttu-id="32b2a-1954">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="32b2a-1954">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="32b2a-1955">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="32b2a-1955">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="32b2a-1956">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="32b2a-1956">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="32b2a-1957">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="32b2a-1957">az vm/vmss disk</span></span>
  3. <span data-ttu-id="32b2a-1958">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1958">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="32b2a-1959">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="32b2a-1959">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="32b2a-1960">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1960">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="32b2a-1961">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-1961">April 3, 2017</span></span>

<span data-ttu-id="32b2a-1962">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="32b2a-1962">Version 2.0.2</span></span>

<span data-ttu-id="32b2a-1963">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-1963">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="32b2a-1964">Core</span><span class="sxs-lookup"><span data-stu-id="32b2a-1964">Core</span></span>

* <span data-ttu-id="32b2a-1965">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="32b2a-1965">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="32b2a-1966">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1966">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="32b2a-1967">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1967">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="32b2a-1968">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1968">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="32b2a-1969">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1969">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="32b2a-1970">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="32b2a-1970">Add prompting for missing template parameters.</span></span> <span data-ttu-id="32b2a-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="32b2a-1972">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1972">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="32b2a-1973">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="32b2a-1973">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="32b2a-1974">ACS</span><span class="sxs-lookup"><span data-stu-id="32b2a-1974">ACS</span></span>

* <span data-ttu-id="32b2a-1975">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1975">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="32b2a-1976">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="32b2a-1976">Add support for ssh key password prompting.</span></span> <span data-ttu-id="32b2a-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="32b2a-1978">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="32b2a-1978">Add support for windows clusters.</span></span> <span data-ttu-id="32b2a-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="32b2a-1980">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="32b2a-1980">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="32b2a-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="32b2a-1982">AppService</span><span class="sxs-lookup"><span data-stu-id="32b2a-1982">AppService</span></span>

* <span data-ttu-id="32b2a-1983">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1983">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="32b2a-1984">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1984">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="32b2a-1985">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1985">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="32b2a-1986">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1986">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="32b2a-1987">DataLake</span><span class="sxs-lookup"><span data-stu-id="32b2a-1987">DataLake</span></span>

* <span data-ttu-id="32b2a-1988">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1988">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="32b2a-1989">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="32b2a-1989">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="32b2a-1990">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="32b2a-1990">DocuemntDB</span></span>

* <span data-ttu-id="32b2a-1991">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1991">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="32b2a-1992">VM</span><span class="sxs-lookup"><span data-stu-id="32b2a-1992">VM</span></span>

* <span data-ttu-id="32b2a-1993">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1993">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="32b2a-1994">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1994">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="32b2a-1995">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1995">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="32b2a-1996">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1996">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="32b2a-1997">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1997">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="32b2a-1998">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1998">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="32b2a-1999">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="32b2a-1999">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="32b2a-2000">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="32b2a-2000">February 27, 2017</span></span>

<span data-ttu-id="32b2a-2001">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="32b2a-2001">Version 2.0.0</span></span>

<span data-ttu-id="32b2a-2002">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="32b2a-2002">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="32b2a-2003">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="32b2a-2003">Container Service (acs)</span></span>
- <span data-ttu-id="32b2a-2004">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="32b2a-2004">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="32b2a-2005">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="32b2a-2005">Networking</span></span>
- <span data-ttu-id="32b2a-2006">Storage</span><span class="sxs-lookup"><span data-stu-id="32b2a-2006">Storage</span></span>

<span data-ttu-id="32b2a-2007">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="32b2a-2007">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="32b2a-2008">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="32b2a-2008">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="32b2a-2009">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="32b2a-2009">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="32b2a-2010">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="32b2a-2010">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="32b2a-2011">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="32b2a-2011">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="32b2a-2012">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="32b2a-2012">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="32b2a-2013">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="32b2a-2013">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="32b2a-2014">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="32b2a-2014">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="32b2a-2015">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="32b2a-2015">Provide feedback from the command line with the `az feedback` command</span></span>


---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/06/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ce11abccc23ee1f150916ef2f91dc895d4664d31
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240509"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="ae124-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ae124-103">Azure CLI release notes</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="ae124-104">6. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-104">May 6, 2019</span></span>

<span data-ttu-id="ae124-105">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="ae124-105">Version 2.0.64</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-106">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-106">Appservice</span></span>
* <span data-ttu-id="ae124-107">`functionapp devops-build`-Befehl als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-107">Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="ae124-108">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="ae124-108">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="ae124-109">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="ae124-109">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="ae124-110">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-110">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="ae124-111">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-111">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="ae124-112">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-112">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="ae124-113">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-113">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="ae124-114">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="ae124-114">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="ae124-115">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-115">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="ae124-116">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-116">Added `create-remote-connection` command</span></span>

### <a name="role"></a><span data-ttu-id="ae124-117">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-117">Role</span></span>
* <span data-ttu-id="ae124-118">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-118">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="ae124-119">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-119">April 23, 2019</span></span>

<span data-ttu-id="ae124-120">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="ae124-120">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-121">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-121">ACS</span></span>
* <span data-ttu-id="ae124-122">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-122">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="ae124-123">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-123">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-124">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-124">AMS</span></span>
* <span data-ttu-id="ae124-125">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-125">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-126">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-126">AppService</span></span>
* <span data-ttu-id="ae124-127">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-127">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="ae124-128">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-128">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="ae124-129">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ae124-129">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="ae124-130">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ae124-130">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="ae124-131">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-131">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="ae124-132">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-132">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="ae124-133">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="ae124-133">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="ae124-134">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="ae124-134">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="ae124-135">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="ae124-135">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="ae124-136">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="ae124-136">Deployment Manager</span></span>
* <span data-ttu-id="ae124-137">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-137">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="ae124-138">Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-138">Lab</span></span>
* <span data-ttu-id="ae124-139">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="ae124-139">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="ae124-140">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-140">Network</span></span>
* <span data-ttu-id="ae124-141">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-141">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-142">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-142">Resource</span></span>
* <span data-ttu-id="ae124-143">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-143">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="ae124-144">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="ae124-144">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="ae124-145">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-145">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="ae124-146">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-146">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-147">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-147">SQL</span></span>
* <span data-ttu-id="ae124-148">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-148">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="ae124-149">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="ae124-149">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="ae124-150">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-150">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="ae124-151">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-151">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-152">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-152">Storage</span></span>
* <span data-ttu-id="ae124-153">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-153">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-154">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-154">VM</span></span>
* <span data-ttu-id="ae124-155">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-155">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="ae124-156">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-156">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="ae124-157">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="ae124-157">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="ae124-158">9. April 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-158">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="ae124-159">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-159">Core</span></span>
* <span data-ttu-id="ae124-160">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-160">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-161">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-161">ACR</span></span>
* <span data-ttu-id="ae124-162">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-162">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-163">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-163">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="ae124-166">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-166">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="ae124-167">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-167">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-168">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-168">AppService</span></span>
* <span data-ttu-id="ae124-169">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-169">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="ae124-170">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-170">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="ae124-171">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-171">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="ae124-172">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="ae124-172">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="ae124-173">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-173">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="ae124-174">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-174">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="ae124-175">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-175">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-176">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-176">CDN</span></span>
* <span data-ttu-id="ae124-177">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="ae124-177">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="ae124-178">Feedback</span><span class="sxs-lookup"><span data-stu-id="ae124-178">Feedback</span></span>
* <span data-ttu-id="ae124-179">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-179">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="ae124-180">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="ae124-180">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="ae124-181">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="ae124-181">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-182">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-182">Monitor</span></span>
* <span data-ttu-id="ae124-183">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="ae124-183">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="ae124-184">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-184">Network</span></span>
* <span data-ttu-id="ae124-185">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-185">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="ae124-186">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-186">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="ae124-187">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-187">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="ae124-188">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="ae124-188">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="ae124-189">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="ae124-189">PrivateDNS</span></span>
* <span data-ttu-id="ae124-190">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-190">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-191">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-191">Resource</span></span>
* <span data-ttu-id="ae124-192">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-192">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="ae124-193">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-193">Role</span></span>
* <span data-ttu-id="ae124-194">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="ae124-194">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="ae124-195">[BREAKING CHANGE] `role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="ae124-195">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-196">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-196">SQL</span></span>
* <span data-ttu-id="ae124-197">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-197">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-198">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-198">Storage</span></span>
* <span data-ttu-id="ae124-199">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-199">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="ae124-200">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="ae124-200">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="ae124-201">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="ae124-201">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="ae124-202">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-202">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="ae124-203">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-203">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="ae124-204">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-204">Core</span></span>
* <span data-ttu-id="ae124-205">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-205">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="ae124-206">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="ae124-206">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="ae124-207">Cloud</span><span class="sxs-lookup"><span data-stu-id="ae124-207">Cloud</span></span>
* <span data-ttu-id="ae124-208">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-208">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-209">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-209">ACR</span></span>
* <span data-ttu-id="ae124-210">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-210">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="ae124-211">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-211">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="ae124-212">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-212">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="ae124-213">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-213">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-214">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-214">AppService</span></span>
* <span data-ttu-id="ae124-215">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-215">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="ae124-216">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-216">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="ae124-217">Bot Service</span><span class="sxs-lookup"><span data-stu-id="ae124-217">BOT Service</span></span>
* <span data-ttu-id="ae124-218">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="ae124-218">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="ae124-219">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-219">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="ae124-220">[BREAKING CHANGE] `--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="ae124-220">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="ae124-221">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-221">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-222">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-222">CDN</span></span>
* <span data-ttu-id="ae124-223">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-223">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="ae124-224">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="ae124-224">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="ae124-225">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ae124-225">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ae124-226">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ae124-226">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-227">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="ae124-227">Cosmosdb</span></span>
* <span data-ttu-id="ae124-228">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-228">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="ae124-229">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-229">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-230">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-230">Interactive</span></span>
* <span data-ttu-id="ae124-231">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-231">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-232">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-232">Monitor</span></span>
* <span data-ttu-id="ae124-233">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="ae124-233">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-234">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-234">Network</span></span>
* <span data-ttu-id="ae124-235">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-235">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-236">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-236">Profile</span></span>
* <span data-ttu-id="ae124-237">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-237">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="ae124-238">Postgres</span><span class="sxs-lookup"><span data-stu-id="ae124-238">Postgres</span></span> 
* <span data-ttu-id="ae124-239">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-239">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="ae124-240">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="ae124-240">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-241">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-241">Resource</span></span>
* <span data-ttu-id="ae124-242">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="ae124-242">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="ae124-243">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-243">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="ae124-244">Graph</span><span class="sxs-lookup"><span data-stu-id="ae124-244">Graph</span></span>
* <span data-ttu-id="ae124-245">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-245">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="ae124-246">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-246">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="ae124-247">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="ae124-247">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="ae124-248">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="ae124-248">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="ae124-249">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-249">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-250">storage</span><span class="sxs-lookup"><span data-stu-id="ae124-250">storage</span></span>
* <span data-ttu-id="ae124-251">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-251">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="ae124-252">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="ae124-252">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="ae124-253">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="ae124-253">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="ae124-254">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-254">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-255">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-255">VM</span></span>
* <span data-ttu-id="ae124-256">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-256">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="ae124-257">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-257">March 12, 2019</span></span>

<span data-ttu-id="ae124-258">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="ae124-258">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="ae124-259">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-259">Core</span></span>

* <span data-ttu-id="ae124-260">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-260">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-261">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-261">ACR</span></span>

* <span data-ttu-id="ae124-262">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-262">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-263">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-263">ACS</span></span>

* <span data-ttu-id="ae124-264">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-264">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="ae124-265">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-265">AppService</span></span>

* <span data-ttu-id="ae124-266">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="ae124-266">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="ae124-267">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-267">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="ae124-268">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="ae124-268">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="ae124-269">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="ae124-269">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="ae124-270">Botservice</span><span class="sxs-lookup"><span data-stu-id="ae124-270">Botservice</span></span>

* <span data-ttu-id="ae124-271">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-271">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="ae124-272">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-272">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="ae124-273">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-273">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="ae124-274">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="ae124-274">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="ae124-275">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-275">Container</span></span>

* <span data-ttu-id="ae124-276">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-276">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="ae124-277">EventHub</span><span class="sxs-lookup"><span data-stu-id="ae124-277">EventHub</span></span>

* <span data-ttu-id="ae124-278">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-278">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="ae124-279">Suchen</span><span class="sxs-lookup"><span data-stu-id="ae124-279">Find</span></span>

* <span data-ttu-id="ae124-280">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="ae124-280">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ae124-281">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ae124-281">HDInsight</span></span>

* <span data-ttu-id="ae124-282">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-282">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="ae124-283">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-283">Network</span></span>

* <span data-ttu-id="ae124-284">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="ae124-284">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-285">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ae124-285">Rdbms</span></span>

* <span data-ttu-id="ae124-286">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="ae124-286">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="ae124-287">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-287">Role</span></span>

* <span data-ttu-id="ae124-288">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="ae124-288">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="ae124-289">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="ae124-289">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ae124-290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ae124-290">Service Fabric</span></span>

* <span data-ttu-id="ae124-291">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-291">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="ae124-292">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-292">February 26, 2019</span></span>

<span data-ttu-id="ae124-293">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="ae124-293">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="ae124-294">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-294">Core</span></span>

* <span data-ttu-id="ae124-295">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="ae124-295">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-296">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-296">ACR</span></span>

* <span data-ttu-id="ae124-297">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-297">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="ae124-298">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="ae124-298">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-299">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-299">ACS</span></span>

* <span data-ttu-id="ae124-300">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-300">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-301">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-301">AppService</span></span>

* <span data-ttu-id="ae124-302">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-302">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-303">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-303">Batch</span></span>
* <span data-ttu-id="ae124-304">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-304">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="ae124-305">[BREAKING CHANGE] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-305">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="ae124-306">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-306">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="ae124-307">[BREAKING CHANGE] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-307">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="ae124-308">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-308">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="ae124-309">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="ae124-309">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-310">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-310">CosmosDB</span></span>

* <span data-ttu-id="ae124-311">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-311">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="ae124-312">Kusto</span><span class="sxs-lookup"><span data-stu-id="ae124-312">Kusto</span></span>

* <span data-ttu-id="ae124-313">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-313">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="ae124-314">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-314">Network</span></span>

* <span data-ttu-id="ae124-315">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-315">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="ae124-316">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-316">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="ae124-317">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-317">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="ae124-318">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-318">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="ae124-319">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-319">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="ae124-320">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-320">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="ae124-321">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-321">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-322">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-322">Resource</span></span>

* <span data-ttu-id="ae124-323">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-323">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="ae124-324">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-324">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="ae124-325">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-325">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="ae124-326">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-326">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="ae124-327">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-327">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="ae124-328">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-328">Role</span></span>

* <span data-ttu-id="ae124-329">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-329">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-330">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-330">VM</span></span>

* <span data-ttu-id="ae124-331">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="ae124-331">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="ae124-332">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-332">February 12, 2019</span></span>

<span data-ttu-id="ae124-333">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="ae124-333">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="ae124-334">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-334">Core</span></span>

* <span data-ttu-id="ae124-335">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-335">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="ae124-336">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-336">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-337">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-337">ACR</span></span>
* <span data-ttu-id="ae124-338">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-338">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="ae124-339">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-339">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-340">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-340">ACS</span></span>
* <span data-ttu-id="ae124-341">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-341">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="ae124-342">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-342">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="ae124-343">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-343">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-344">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-344">AMS</span></span>
* <span data-ttu-id="ae124-345">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-345">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="ae124-346">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-346">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-347">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-347">Appservice</span></span>
* <span data-ttu-id="ae124-348">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-348">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="ae124-349">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-349">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="ae124-350">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="ae124-350">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="ae124-351">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-351">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="ae124-352">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-352">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="ae124-353">Botservice</span><span class="sxs-lookup"><span data-stu-id="ae124-353">Botservice</span></span>
* <span data-ttu-id="ae124-354">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="ae124-354">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="ae124-355">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-355">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="ae124-356">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-356">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="ae124-357">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="ae124-357">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="ae124-358">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-358">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="ae124-359">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="ae124-359">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="ae124-360">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-360">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="ae124-361">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-361">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="ae124-362">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="ae124-362">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="ae124-363">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="ae124-363">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="ae124-364">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ae124-364">Key Vault</span></span>
* <span data-ttu-id="ae124-365">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="ae124-365">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-366">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-366">Monitor</span></span>
* <span data-ttu-id="ae124-367">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-367">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-368">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-368">Network</span></span>
* <span data-ttu-id="ae124-369">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="ae124-369">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="ae124-370">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae124-370">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="ae124-371">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae124-371">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="ae124-372">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-372">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ae124-373">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="ae124-373">Policy Insights</span></span>
* <span data-ttu-id="ae124-374">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae124-374">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-375">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-375">RDBMS</span></span>
* <span data-ttu-id="ae124-376">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="ae124-376">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="ae124-377">Redis</span><span class="sxs-lookup"><span data-stu-id="ae124-377">Redis</span></span>
* <span data-ttu-id="ae124-378">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-378">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="ae124-379">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-379">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="ae124-380">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-380">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="ae124-381">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-381">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="ae124-382">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-382">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="ae124-383">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-383">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="ae124-384">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-384">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="ae124-385">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-385">Role</span></span>
* <span data-ttu-id="ae124-386">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-386">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="ae124-387">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="ae124-387">SQL VM</span></span>
* <span data-ttu-id="ae124-388">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-388">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-389">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-389">VM</span></span>
* <span data-ttu-id="ae124-390">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="ae124-390">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="ae124-391">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-391">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="ae124-392">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="ae124-392">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="ae124-393">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-393">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="ae124-394">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-394">January 31, 2019</span></span>

<span data-ttu-id="ae124-395">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="ae124-395">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="ae124-396">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-396">Core</span></span>

* <span data-ttu-id="ae124-397">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="ae124-397">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="ae124-398">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-398">January 28, 2019</span></span>

<span data-ttu-id="ae124-399">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="ae124-399">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-400">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-400">ACR</span></span>
* <span data-ttu-id="ae124-401">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-401">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-402">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-402">ACS</span></span>
* <span data-ttu-id="ae124-403">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-403">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="ae124-404">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-404">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="ae124-405">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-405">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-406">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-406">AMS</span></span>
* <span data-ttu-id="ae124-407">[BREAKING CHANGE] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-407">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="ae124-408">[BREAKING CHANGE] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-408">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-409">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-409">Appservice</span></span>
* <span data-ttu-id="ae124-410">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-410">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="ae124-411">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-411">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="ae124-412">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-412">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="ae124-413">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-413">Container</span></span>
* <span data-ttu-id="ae124-414">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-414">Added `container start` command</span></span>
* <span data-ttu-id="ae124-415">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="ae124-415">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ae124-416">EventGrid</span><span class="sxs-lookup"><span data-stu-id="ae124-416">EventGrid</span></span>
* <span data-ttu-id="ae124-417">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-417">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="ae124-418">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-418">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="ae124-419">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-419">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="ae124-420">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-420">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="ae124-421">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-421">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ae124-422">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ae124-422">HDInsight</span></span>
* <span data-ttu-id="ae124-423">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-423">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="ae124-424">[BREAKING CHANGE] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-424">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="ae124-425">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-425">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="ae124-426">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-426">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="ae124-427">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-427">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="ae124-428">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-428">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-429">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-429">IoT</span></span>
* <span data-ttu-id="ae124-430">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-430">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="ae124-431">Kusto</span><span class="sxs-lookup"><span data-stu-id="ae124-431">Kusto</span></span>
* <span data-ttu-id="ae124-432">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="ae124-432">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-433">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-433">Monitor</span></span>
* <span data-ttu-id="ae124-434">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-434">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-435">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-435">Profile</span></span>
* <span data-ttu-id="ae124-436">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ae124-436">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-437">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-437">Network</span></span>
* <span data-ttu-id="ae124-438">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="ae124-438">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="ae124-439">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="ae124-439">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-440">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-440">Resource</span></span>
* <span data-ttu-id="ae124-441">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-441">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="ae124-442">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-442">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="ae124-443">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="ae124-443">SQL Virtual Machine</span></span>
* <span data-ttu-id="ae124-444">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="ae124-444">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-445">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-445">Storage</span></span>
* <span data-ttu-id="ae124-446">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-446">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="ae124-447">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-447">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-448">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-448">VM</span></span>
* <span data-ttu-id="ae124-449">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-449">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="ae124-450">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-450">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="ae124-451">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="ae124-451">January 15, 2019</span></span>

<span data-ttu-id="ae124-452">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="ae124-452">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-453">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-453">ACR</span></span>
* <span data-ttu-id="ae124-454">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-454">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="ae124-455">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-455">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="ae124-456">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="ae124-456">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="ae124-457">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-457">ACS</span></span>
* <span data-ttu-id="ae124-458">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-458">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-459">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-459">Appservice</span></span>
* <span data-ttu-id="ae124-460">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="ae124-460">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="ae124-461">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-461">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="ae124-462">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-462">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="ae124-463">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-463">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="ae124-464">Botservice</span><span class="sxs-lookup"><span data-stu-id="ae124-464">Botservice</span></span>
* <span data-ttu-id="ae124-465">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-465">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="ae124-466">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="ae124-466">Configure</span></span>
* <span data-ttu-id="ae124-467">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-467">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-468">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-468">CosmosDB</span></span>
* <span data-ttu-id="ae124-469">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-469">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ae124-470">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ae124-470">HDInsight</span></span>
* <span data-ttu-id="ae124-471">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-471">Added commands for managing applications</span></span>
* <span data-ttu-id="ae124-472">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-472">Added commands for managing script actions</span></span>
* <span data-ttu-id="ae124-473">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-473">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="ae124-474">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-474">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="ae124-475">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-475">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-476">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-476">Network</span></span>
* <span data-ttu-id="ae124-477">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-477">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="ae124-478">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="ae124-478">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="ae124-479">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-479">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="ae124-480">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="ae124-480">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="ae124-481">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-481">Role</span></span>
* <span data-ttu-id="ae124-482">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ae124-482">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="ae124-483">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="ae124-483">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="ae124-484">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="ae124-484">Security</span></span>
* <span data-ttu-id="ae124-485">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-485">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-486">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-486">Storage</span></span>
* <span data-ttu-id="ae124-487">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="ae124-487">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="ae124-488">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-488">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="ae124-489">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-489">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="ae124-490">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-490">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="ae124-491">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-491">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-492">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-492">VM</span></span>
* <span data-ttu-id="ae124-493">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="ae124-493">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="ae124-494">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-494">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ae124-495">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-495">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="ae124-496">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="ae124-496">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="ae124-497">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="ae124-497">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="ae124-498">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="ae124-498">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="ae124-499">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-499">December 20, 2018</span></span>

<span data-ttu-id="ae124-500">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="ae124-500">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="ae124-501">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-501">Appservice</span></span>
* <span data-ttu-id="ae124-502">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-502">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="ae124-503">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-503">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="ae124-504">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-504">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ae124-505">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="ae124-505">IoTCentral</span></span>
* <span data-ttu-id="ae124-506">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-506">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="ae124-507">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-507">Role</span></span>
* <span data-ttu-id="ae124-508">[BREAKING CHANGE] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="ae124-508">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-509">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-509">SQL</span></span>
* <span data-ttu-id="ae124-510">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-510">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-511">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-511">VM</span></span>
* <span data-ttu-id="ae124-512">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-512">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="ae124-513">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-513">December 18, 2018</span></span>

<span data-ttu-id="ae124-514">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="ae124-514">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="ae124-515">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-515">ACR</span></span>
* <span data-ttu-id="ae124-516">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-516">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="ae124-517">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="ae124-517">Condensed the table layout for task list</span></span>
* <span data-ttu-id="ae124-518">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-518">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-519">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-519">ACS</span></span>
* <span data-ttu-id="ae124-520">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-520">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="ae124-521">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-521">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="ae124-522">[VERALTET] `az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-522">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="ae124-523">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="ae124-523">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="ae124-524">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-524">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="ae124-525">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-525">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-526">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-526">Appservice</span></span>
* <span data-ttu-id="ae124-527">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-527">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="ae124-528">Botservice</span><span class="sxs-lookup"><span data-stu-id="ae124-528">Botservice</span></span>
* <span data-ttu-id="ae124-529">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-529">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="ae124-530">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-530">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="ae124-531">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-531">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="ae124-532">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="ae124-532">Reduced Kudu network calls</span></span>
* <span data-ttu-id="ae124-533">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="ae124-533">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-534">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-534">Consumption</span></span>
* <span data-ttu-id="ae124-535">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-535">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-536">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-536">CosmosDB</span></span>
* <span data-ttu-id="ae124-537">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-537">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="ae124-538">Karten</span><span class="sxs-lookup"><span data-stu-id="ae124-538">Maps</span></span>
* <span data-ttu-id="ae124-539">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-539">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-540">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-540">Network</span></span>
* <span data-ttu-id="ae124-541">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-541">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="ae124-542">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="ae124-542">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-543">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-543">Resource</span></span>
* <span data-ttu-id="ae124-544">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-544">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="ae124-545">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-545">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-546">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-546">Storage</span></span>
*  <span data-ttu-id="ae124-547">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-547">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-548">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-548">VM</span></span>
* <span data-ttu-id="ae124-549">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="ae124-549">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="ae124-550">4. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-550">December 4, 2018</span></span>

<span data-ttu-id="ae124-551">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="ae124-551">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="ae124-552">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-552">Core</span></span>
* <span data-ttu-id="ae124-553">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-553">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="ae124-554">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-554">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-555">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-555">Appservice</span></span>
* <span data-ttu-id="ae124-556">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae124-556">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="ae124-557">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="ae124-557">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="ae124-558">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-558">Network</span></span>
* <span data-ttu-id="ae124-559">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-559">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="ae124-560">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-560">Role</span></span>
* <span data-ttu-id="ae124-561">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-561">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="ae124-562">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-562">VM</span></span>
* <span data-ttu-id="ae124-563">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-563">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="ae124-564">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="ae124-564">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="ae124-565">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="ae124-565">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="ae124-566">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="ae124-566">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="ae124-567">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-567">November 20, 2018</span></span>

<span data-ttu-id="ae124-568">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="ae124-568">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="ae124-569">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-569">Core</span></span>
* <span data-ttu-id="ae124-570">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-570">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-571">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-571">ACR</span></span>
* <span data-ttu-id="ae124-572">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-572">Added context token to task step</span></span>
* <span data-ttu-id="ae124-573">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-573">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="ae124-574">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-574">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-575">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-575">Appservice</span></span>
* <span data-ttu-id="ae124-576">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-576">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="ae124-577">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="ae124-577">Updated the default `node_version`.</span></span> <span data-ttu-id="ae124-578">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="ae124-578">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="ae124-579">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-579">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="ae124-580">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="ae124-580">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ae124-581">IotCentral</span><span class="sxs-lookup"><span data-stu-id="ae124-581">IotCentral</span></span>
* <span data-ttu-id="ae124-582">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-582">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-583">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-583">KeyVault</span></span>
* <span data-ttu-id="ae124-584">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-584">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="ae124-585">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-585">Network</span></span>
* <span data-ttu-id="ae124-586">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-586">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="ae124-587">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-587">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="ae124-588">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-588">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="ae124-589">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-589">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-590">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ae124-590">Rdbms</span></span>
* <span data-ttu-id="ae124-591">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-591">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="ae124-592">RBAC</span><span class="sxs-lookup"><span data-stu-id="ae124-592">Rbac</span></span>
* <span data-ttu-id="ae124-593">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-593">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="ae124-594">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-594">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="ae124-595">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-595">Storage</span></span>
* <span data-ttu-id="ae124-596">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-596">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="ae124-597">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="ae124-597">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="ae124-598">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-598">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="ae124-599">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-599">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-600">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-600">VM</span></span>
* <span data-ttu-id="ae124-601">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-601">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="ae124-602">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-602">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="ae124-603">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="ae124-603">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="ae124-604">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-604">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="ae124-605">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-605">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="ae124-606">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-606">Added `snapshot wait` command</span></span>
* <span data-ttu-id="ae124-607">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-607">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="ae124-608">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-608">November 6, 2018</span></span>

<span data-ttu-id="ae124-609">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="ae124-609">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="ae124-610">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-610">Core</span></span>
* <span data-ttu-id="ae124-611">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-611">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-612">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-612">ACR</span></span>
* <span data-ttu-id="ae124-613">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-613">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="ae124-614">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-614">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-615">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-615">ACS</span></span>
* <span data-ttu-id="ae124-616">[BREAKING CHANGE] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="ae124-616">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="ae124-617">Advisor</span><span class="sxs-lookup"><span data-stu-id="ae124-617">Advisor</span></span>
* <span data-ttu-id="ae124-618">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="ae124-618">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-619">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-619">AMS</span></span>
* <span data-ttu-id="ae124-620">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-620">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="ae124-621">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-621">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="ae124-622">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-622">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="ae124-623">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-623">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="ae124-624">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-624">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="ae124-625">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-625">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="ae124-626">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-626">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="ae124-627">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="ae124-627">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="ae124-628">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-628">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="ae124-629">[BREAKING CHANGE] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-629">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="ae124-630">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="ae124-630">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="ae124-631">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ae124-631">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="ae124-632">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="ae124-632">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="ae124-633">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-633">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="ae124-634">[BREAKING CHANGE] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="ae124-634">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="ae124-635">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-635">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="ae124-636">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="ae124-636">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-637">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-637">AppService</span></span>
* <span data-ttu-id="ae124-638">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="ae124-638">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="ae124-639">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="ae124-639">Configure</span></span>
* <span data-ttu-id="ae124-640">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-640">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="ae124-641">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-641">Container</span></span>
* <span data-ttu-id="ae124-642">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="ae124-642">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="ae124-643">EventHub</span><span class="sxs-lookup"><span data-stu-id="ae124-643">EventHub</span></span>
* <span data-ttu-id="ae124-644">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-644">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-645">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-645">Interactive</span></span>
* <span data-ttu-id="ae124-646">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-646">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-647">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-647">Monitor</span></span>
* <span data-ttu-id="ae124-648">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-648">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-649">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-649">Network</span></span>
* <span data-ttu-id="ae124-650">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-650">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="ae124-651">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="ae124-651">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="ae124-652">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="ae124-652">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="ae124-653">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-653">Profile</span></span>
* <span data-ttu-id="ae124-654">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-654">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-655">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-655">RDBMS</span></span>
* <span data-ttu-id="ae124-656">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-656">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-657">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-657">Resource</span></span>
* <span data-ttu-id="ae124-658">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-658">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="ae124-659">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-659">Role</span></span>
* <span data-ttu-id="ae124-660">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-660">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="ae124-661">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="ae124-661">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="ae124-662">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-662">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-663">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-663">Storage</span></span>
* <span data-ttu-id="ae124-664">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="ae124-664">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-665">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-665">VM</span></span>
* <span data-ttu-id="ae124-666">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-666">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="ae124-667">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="ae124-667">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="ae124-668">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-668">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="ae124-669">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="ae124-669">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="ae124-670">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-670">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="ae124-671">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-671">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="ae124-672">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-672">October 23, 2018</span></span>

<span data-ttu-id="ae124-673">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="ae124-673">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="ae124-674">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-674">Core</span></span>
* <span data-ttu-id="ae124-675">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="ae124-675">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="ae124-676">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="ae124-676">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-677">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-677">ACR</span></span>
* <span data-ttu-id="ae124-678">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-678">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-679">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-679">CDN</span></span>
* <span data-ttu-id="ae124-680">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-680">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ae124-681">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ae124-681">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="ae124-682">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-682">Container</span></span>
* <span data-ttu-id="ae124-683">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-683">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="ae124-684">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="ae124-684">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="ae124-685">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-685">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="ae124-686">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="ae124-686">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="ae124-687">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="ae124-687">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="ae124-688">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-688">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="ae124-689">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-689">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-690">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-690">CosmosDB</span></span>
* <span data-ttu-id="ae124-691">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-691">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-692">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-692">Interactive</span></span>
* <span data-ttu-id="ae124-693">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-693">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="ae124-694">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ae124-694">IoT Central</span></span>
* <span data-ttu-id="ae124-695">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-695">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="ae124-696">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="ae124-696">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-697">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-697">Monitor</span></span>
* <span data-ttu-id="ae124-698">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="ae124-698">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="ae124-699">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-699">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="ae124-700">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-700">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ae124-701">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-701">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="ae124-702">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-702">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="ae124-703">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-703">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="ae124-704">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="ae124-704">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="ae124-705">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-705">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ae124-706">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-706">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="ae124-707">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-707">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-708">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-708">Network</span></span>
* <span data-ttu-id="ae124-709">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-709">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="ae124-710">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-710">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="ae124-711">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ae124-711">ServiceBus</span></span>
* <span data-ttu-id="ae124-712">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-712">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-713">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-713">SQL</span></span>
* <span data-ttu-id="ae124-714">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="ae124-714">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-715">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-715">Storage</span></span>
* <span data-ttu-id="ae124-716">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-716">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="ae124-717">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-717">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-718">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-718">VM</span></span>
* <span data-ttu-id="ae124-719">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="ae124-719">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="ae124-720">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-720">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="ae124-721">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-721">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="ae124-722">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-722">October 16, 2018</span></span>

<span data-ttu-id="ae124-723">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="ae124-723">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-724">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-724">VM</span></span>
* <span data-ttu-id="ae124-725">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="ae124-725">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="ae124-726">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-726">October 9, 2018</span></span>

<span data-ttu-id="ae124-727">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="ae124-727">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="ae124-728">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-728">Core</span></span>
* <span data-ttu-id="ae124-729">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="ae124-729">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-730">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-730">ACR</span></span>
* <span data-ttu-id="ae124-731">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-731">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-732">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-732">ACS</span></span>
* <span data-ttu-id="ae124-733">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="ae124-733">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="ae124-734">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="ae124-734">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="ae124-735">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="ae124-735">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="ae124-736">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="ae124-736">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="ae124-737">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-737">Container</span></span>
* <span data-ttu-id="ae124-738">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-738">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="ae124-739">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-739">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="ae124-740">Event Hub</span><span class="sxs-lookup"><span data-stu-id="ae124-740">Event Hub</span></span>
* <span data-ttu-id="ae124-741">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-741">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="ae124-742">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-742">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="ae124-743">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ae124-743">Extensions</span></span>
* <span data-ttu-id="ae124-744">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="ae124-744">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ae124-745">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ae124-745">HDInsight</span></span>
* <span data-ttu-id="ae124-746">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-746">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-747">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-747">IoT</span></span>
* <span data-ttu-id="ae124-748">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-748">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-749">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-749">KeyVault</span></span>
* <span data-ttu-id="ae124-750">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="ae124-750">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="ae124-751">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-751">Network</span></span>
* <span data-ttu-id="ae124-752">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="ae124-752">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="ae124-753">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="ae124-753">See #6052</span></span>
* <span data-ttu-id="ae124-754">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="ae124-754">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="ae124-755">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="ae124-755">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="ae124-756">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-756">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="ae124-757">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-757">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="ae124-758">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="ae124-758">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="ae124-759">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-759">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="ae124-760">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-760">Role</span></span>
* <span data-ttu-id="ae124-761">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-761">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="ae124-762">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-762">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="ae124-763">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ae124-763">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="ae124-764">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="ae124-764">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="ae124-765">Service Bus</span><span class="sxs-lookup"><span data-stu-id="ae124-765">Service Bus</span></span>
* <span data-ttu-id="ae124-766">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-766">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-767">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-767">VM</span></span>
* <span data-ttu-id="ae124-768">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-768">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="ae124-769">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="ae124-769">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="ae124-770">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-770">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="ae124-771">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-771">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="ae124-772">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-772">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="ae124-773">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-773">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="ae124-774">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-774">September 21, 2018</span></span>

<span data-ttu-id="ae124-775">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="ae124-775">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-776">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-776">ACR</span></span>
* <span data-ttu-id="ae124-777">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-777">Added ACR Task commands</span></span>
* <span data-ttu-id="ae124-778">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-778">Added quick run command</span></span>
* <span data-ttu-id="ae124-779">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-779">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="ae124-780">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-780">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="ae124-781">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-781">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="ae124-782">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-782">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-783">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-783">ACS</span></span>
* <span data-ttu-id="ae124-784">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-784">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="ae124-785">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-785">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-786">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-786">AppService</span></span>

* <span data-ttu-id="ae124-787">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="ae124-787">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="ae124-788">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-788">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="ae124-789">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-789">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="ae124-790">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-790">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-791">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-791">Batch</span></span>
* <span data-ttu-id="ae124-792">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-792">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="ae124-793">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-793">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="ae124-794">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-794">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="ae124-795">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-795">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ae124-796">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-796">Batch AI</span></span> 
* <span data-ttu-id="ae124-797">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-797">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ae124-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ae124-798">Cognitive Services</span></span>
* <span data-ttu-id="ae124-799">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-799">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="ae124-800">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-800">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="ae124-801">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-801">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="ae124-802">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-802">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="ae124-803">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-803">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="ae124-804">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="ae124-804">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="ae124-805">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-805">Container</span></span>
* <span data-ttu-id="ae124-806">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-806">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="ae124-807">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-807">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="ae124-808">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-808">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="ae124-809">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-809">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="ae124-810">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ae124-810">Datalake</span></span>
* <span data-ttu-id="ae124-811">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-811">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="ae124-812">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="ae124-812">Interactive Shell</span></span>
* <span data-ttu-id="ae124-813">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-813">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="ae124-814">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-814">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-815">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-815">IoT</span></span>
* <span data-ttu-id="ae124-816">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-816">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="ae124-817">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ae124-817">Key Vault</span></span>
* <span data-ttu-id="ae124-818">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-818">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="ae124-819">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-819">Network</span></span>
* <span data-ttu-id="ae124-820">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-820">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="ae124-821">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-821">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="ae124-822">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-822">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="ae124-823">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-823">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="ae124-824">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-824">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="ae124-825">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-825">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="ae124-826">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-826">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="ae124-827">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="ae124-827">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="ae124-828">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-828">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="ae124-829">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-829">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="ae124-830">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-830">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="ae124-831">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-831">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="ae124-832">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-832">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="ae124-833">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="ae124-833">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="ae124-834">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-834">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="ae124-835">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="ae124-835">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="ae124-836">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-836">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="ae124-837">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-837">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-838">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-838">RDBMS</span></span>
* <span data-ttu-id="ae124-839">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-839">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="ae124-840">Reservierung</span><span class="sxs-lookup"><span data-stu-id="ae124-840">Reservation</span></span>
* <span data-ttu-id="ae124-841">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-841">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="ae124-842">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-842">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="ae124-843">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="ae124-843">Manage App</span></span>
* <span data-ttu-id="ae124-844">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="ae124-844">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="ae124-845">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="ae124-845">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="ae124-846">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-846">Role</span></span>
* <span data-ttu-id="ae124-847">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-847">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="ae124-848">SignalR</span><span class="sxs-lookup"><span data-stu-id="ae124-848">SignalR</span></span>
* <span data-ttu-id="ae124-849">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-849">First release</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-850">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-850">Storage</span></span>
* <span data-ttu-id="ae124-851">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-851">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="ae124-852">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-852">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-853">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-853">VM</span></span>
* <span data-ttu-id="ae124-854">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="ae124-854">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="ae124-855">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-855">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="ae124-856">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-856">August 28, 2018</span></span>

<span data-ttu-id="ae124-857">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="ae124-857">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="ae124-858">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-858">Core</span></span>

* <span data-ttu-id="ae124-859">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-859">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="ae124-860">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-860">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-861">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-861">ACR</span></span>

* <span data-ttu-id="ae124-862">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-862">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="ae124-863">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="ae124-863">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-864">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-864">ACS</span></span>

* <span data-ttu-id="ae124-865">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-865">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="ae124-866">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="ae124-866">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-867">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-867">AppService</span></span>

* <span data-ttu-id="ae124-868">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-868">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="ae124-869">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-869">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="ae124-870">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-870">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="ae124-871">Backup</span><span class="sxs-lookup"><span data-stu-id="ae124-871">Backup</span></span>

* <span data-ttu-id="ae124-872">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-872">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="ae124-873">Botdienst</span><span class="sxs-lookup"><span data-stu-id="ae124-873">Bot Service</span></span>

* <span data-ttu-id="ae124-874">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="ae124-874">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ae124-875">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ae124-875">Cognitive Services</span></span>

* <span data-ttu-id="ae124-876">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="ae124-876">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-877">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-877">IoT</span></span>

* <span data-ttu-id="ae124-878">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-878">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-879">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-879">Monitor</span></span>

* <span data-ttu-id="ae124-880">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-880">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="ae124-881">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-881">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ae124-882">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-882">Network</span></span>

* <span data-ttu-id="ae124-883">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-883">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-884">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-884">Resource</span></span>

* <span data-ttu-id="ae124-885">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-885">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-886">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-886">Storage</span></span>

* <span data-ttu-id="ae124-887">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-887">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-888">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-888">VM</span></span>

* <span data-ttu-id="ae124-889">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="ae124-889">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="ae124-890">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="ae124-890">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="ae124-891">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-891">Auguest 14, 2018</span></span>

<span data-ttu-id="ae124-892">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="ae124-892">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="ae124-893">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-893">Core</span></span>

* <span data-ttu-id="ae124-894">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-894">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="ae124-895">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-895">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="ae124-896">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="ae124-896">Telemetry</span></span>

* <span data-ttu-id="ae124-897">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="ae124-897">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-898">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-898">ACR</span></span>

* <span data-ttu-id="ae124-899">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-899">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="ae124-900">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-900">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-901">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-901">ACS</span></span>

* <span data-ttu-id="ae124-902">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-902">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="ae124-903">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="ae124-903">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="ae124-904">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="ae124-904">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="ae124-905">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="ae124-905">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="ae124-906">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="ae124-906">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="ae124-907">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-907">AppService</span></span>

* <span data-ttu-id="ae124-908">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="ae124-908">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="ae124-909">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-909">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="ae124-910">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-910">BatchAI</span></span>

* <span data-ttu-id="ae124-911">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="ae124-911">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="ae124-912">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-912">Container</span></span>

* <span data-ttu-id="ae124-913">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-913">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="ae124-914">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-914">IoT</span></span>

* <span data-ttu-id="ae124-915">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-915">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="ae124-916">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="ae124-916">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="ae124-917">Iot Central</span><span class="sxs-lookup"><span data-stu-id="ae124-917">Iot Central</span></span>

* <span data-ttu-id="ae124-918">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-918">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-919">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-919">KeyVault</span></span>


* <span data-ttu-id="ae124-920">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-920">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="ae124-921">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-921">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="ae124-922">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-922">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="ae124-923">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-923">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="ae124-924">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-924">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="ae124-925">Relay</span><span class="sxs-lookup"><span data-stu-id="ae124-925">Relay</span></span>

* <span data-ttu-id="ae124-926">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-926">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-927">Sql</span><span class="sxs-lookup"><span data-stu-id="ae124-927">Sql</span></span>

* <span data-ttu-id="ae124-928">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-928">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-929">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-929">Storage</span></span>

* <span data-ttu-id="ae124-930">[BREAKING CHANGE] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="ae124-930">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="ae124-931">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="ae124-931">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="ae124-932">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-932">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="ae124-933">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="ae124-933">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="ae124-934">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="ae124-934">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-935">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-935">VM</span></span>

* <span data-ttu-id="ae124-936">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-936">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="ae124-937">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-937">July 31, 2018</span></span>

<span data-ttu-id="ae124-938">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="ae124-938">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-939">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-939">ACR</span></span>

* <span data-ttu-id="ae124-940">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-940">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="ae124-941">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-941">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-942">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-942">ACS</span></span>

* <span data-ttu-id="ae124-943">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-943">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-944">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-944">Batch</span></span>

* <span data-ttu-id="ae124-945">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="ae124-945">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="ae124-946">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-946">Container</span></span>

* <span data-ttu-id="ae124-947">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-947">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="ae124-948">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-948">Network</span></span>

* <span data-ttu-id="ae124-949">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-949">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="ae124-950">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-950">Resource</span></span>

* <span data-ttu-id="ae124-951">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="ae124-951">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="ae124-952">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="ae124-952">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="ae124-953">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-953">Role</span></span>

* <span data-ttu-id="ae124-954">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-954">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="ae124-955">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="ae124-955">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="ae124-956">Suchen,</span><span class="sxs-lookup"><span data-stu-id="ae124-956">Search</span></span>

* <span data-ttu-id="ae124-957">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-957">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="ae124-958">Service Bus</span><span class="sxs-lookup"><span data-stu-id="ae124-958">Service Bus</span></span>

* <span data-ttu-id="ae124-959">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="ae124-959">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="ae124-960">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-960">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="ae124-961">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="ae124-961">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="ae124-962">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="ae124-962">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-963">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-963">Storage</span></span>

* <span data-ttu-id="ae124-964">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-964">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="ae124-965">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-965">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-966">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-966">VM</span></span>

* <span data-ttu-id="ae124-967">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-967">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="ae124-968">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-968">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="ae124-969">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-969">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="ae124-970">[BREAKING CHANGE] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-970">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="ae124-971">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-971">July 18, 2018</span></span>

<span data-ttu-id="ae124-972">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="ae124-972">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="ae124-973">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-973">Core</span></span>

* <span data-ttu-id="ae124-974">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-974">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="ae124-975">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-975">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="ae124-976">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="ae124-976">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-977">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-977">ACR</span></span>

* <span data-ttu-id="ae124-978">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-978">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="ae124-979">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-979">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="ae124-980">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-980">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="ae124-981">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-981">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-982">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-982">ACS</span></span>

* <span data-ttu-id="ae124-983">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="ae124-983">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-984">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-984">AppService</span></span>

* <span data-ttu-id="ae124-985">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-985">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-986">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-986">Batch</span></span>

* <span data-ttu-id="ae124-987">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="ae124-987">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="ae124-988">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-988">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ae124-989">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-989">Batch AI</span></span>

* <span data-ttu-id="ae124-990">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-990">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="ae124-991">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-991">Container</span></span>

* <span data-ttu-id="ae124-992">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-992">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="ae124-993">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-993">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="ae124-994">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-994">Network</span></span>

* <span data-ttu-id="ae124-995">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-995">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="ae124-996">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-996">Added `network nic wait`</span></span>
* <span data-ttu-id="ae124-997">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-997">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="ae124-998">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="ae124-998">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="ae124-999">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-999">Resource</span></span>

* <span data-ttu-id="ae124-1000">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1000">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="ae124-1001">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1001">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="ae124-1002">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1002">Added `deployment wait` command</span></span>
* <span data-ttu-id="ae124-1003">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1003">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1004">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1004">SQL</span></span>

* <span data-ttu-id="ae124-1005">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1005">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="ae124-1006">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="ae124-1006">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="ae124-1007">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1007">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1008">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1008">Storage</span></span>

* <span data-ttu-id="ae124-1009">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1009">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1010">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1010">VM</span></span>

* <span data-ttu-id="ae124-1011">[BREAKING CHANGE] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1011">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="ae124-1012">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1012">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="ae124-1013">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1013">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ae124-1014">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1014">July 3, 2018</span></span>

<span data-ttu-id="ae124-1015">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="ae124-1015">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="ae124-1016">AKS</span><span class="sxs-lookup"><span data-stu-id="ae124-1016">AKS</span></span>

* <span data-ttu-id="ae124-1017">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1017">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ae124-1018">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1018">July 3, 2018</span></span>

<span data-ttu-id="ae124-1019">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="ae124-1019">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1020">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1020">Core</span></span>

* <span data-ttu-id="ae124-1021">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1021">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1022">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1022">ACR</span></span>

* <span data-ttu-id="ae124-1023">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1023">Added polling build status</span></span>
* <span data-ttu-id="ae124-1024">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1024">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="ae124-1025">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1025">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1026">ACS</span></span>

* <span data-ttu-id="ae124-1027">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ae124-1027">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="ae124-1028">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="ae124-1028">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="ae124-1029">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1029">Updated options for `aks browse` command.</span></span> <span data-ttu-id="ae124-1030">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1030">Added `--listen-port` support</span></span>
* <span data-ttu-id="ae124-1031">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1031">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="ae124-1032">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="ae124-1032">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="ae124-1033">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1033">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1034">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1034">AppService</span></span>

* <span data-ttu-id="ae124-1035">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1035">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="ae124-1036">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1036">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="ae124-1037">Backup</span><span class="sxs-lookup"><span data-stu-id="ae124-1037">Backup</span></span>

* <span data-ttu-id="ae124-1038">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1038">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="ae124-1039">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-1039">BatchAI</span></span>

* <span data-ttu-id="ae124-1040">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1040">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="ae124-1041">Cloud</span><span class="sxs-lookup"><span data-stu-id="ae124-1041">Cloud</span></span>

* <span data-ttu-id="ae124-1042">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1042">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1043">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1043">Container</span></span>

* <span data-ttu-id="ae124-1044">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1044">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="ae124-1045">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1045">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="ae124-1046">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1046">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1047">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1047">Extension</span></span>

* <span data-ttu-id="ae124-1048">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1048">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1049">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1049">Network</span></span>

* <span data-ttu-id="ae124-1050">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="ae124-1050">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-1051">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ae124-1051">Rdbms</span></span>

* <span data-ttu-id="ae124-1052">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1052">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1053">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1053">Resource</span></span>

* <span data-ttu-id="ae124-1054">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1054">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1055">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1055">VM</span></span>

* <span data-ttu-id="ae124-1056">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1056">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="ae124-1057">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1057">June 25, 2018</span></span>

<span data-ttu-id="ae124-1058">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="ae124-1058">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="ae124-1059">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="ae124-1059">CLI</span></span>

* <span data-ttu-id="ae124-1060">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="ae124-1060">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="ae124-1061">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1061">June 19, 2018</span></span>

<span data-ttu-id="ae124-1062">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="ae124-1062">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1063">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1063">Core</span></span>

* <span data-ttu-id="ae124-1064">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1064">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1065">ACR</span></span>

* <span data-ttu-id="ae124-1066">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1066">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="ae124-1067">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1067">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1068">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1068">ACS</span></span>

* <span data-ttu-id="ae124-1069">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1069">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="ae124-1070">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1070">Added `--update` support</span></span>
* <span data-ttu-id="ae124-1071">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1071">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="ae124-1072">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-1072">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="ae124-1073">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1073">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="ae124-1074">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="ae124-1074">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="ae124-1075">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1075">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="ae124-1076">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1076">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1077">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1077">AppService</span></span>

* <span data-ttu-id="ae124-1078">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1078">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="ae124-1079">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1079">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-1080">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-1080">Batch</span></span>

* <span data-ttu-id="ae124-1081">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1081">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ae124-1082">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-1082">Batch AI</span></span>

* <span data-ttu-id="ae124-1083">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1083">Added support for workspaces.</span></span> <span data-ttu-id="ae124-1084">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="ae124-1084">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="ae124-1085">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1085">Added support for experiments.</span></span> <span data-ttu-id="ae124-1086">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1086">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="ae124-1087">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1087">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="ae124-1088">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1088">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="ae124-1089">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="ae124-1089">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="ae124-1090">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1090">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="ae124-1091">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-1091">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="ae124-1092">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-1092">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="ae124-1093">[BREAKING CHANGE] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1093">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="ae124-1094">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="ae124-1094">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="ae124-1095">[BREAKING CHANGE] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1095">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="ae124-1096">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="ae124-1096">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="ae124-1097">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1097">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="ae124-1098">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="ae124-1098">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="ae124-1099">[BREAKING CHANGE] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1099">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="ae124-1100">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="ae124-1100">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="ae124-1101">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1101">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="ae124-1102">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1102">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ae124-1103">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1103">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ae124-1104">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1104">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="ae124-1105">Karten</span><span class="sxs-lookup"><span data-stu-id="ae124-1105">Maps</span></span>

* <span data-ttu-id="ae124-1106">[BREAKING CHANGE] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1106">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1107">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1107">Network</span></span>

* <span data-ttu-id="ae124-1108">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="ae124-1108">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="ae124-1109">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="ae124-1109">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="ae124-1110">#6502</span><span class="sxs-lookup"><span data-stu-id="ae124-1110">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="ae124-1111">Reservations</span><span class="sxs-lookup"><span data-stu-id="ae124-1111">Reservations</span></span>

* <span data-ttu-id="ae124-1112">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1112">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="ae124-1113">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1113">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="ae124-1114">[BREAKING CHANGE] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1114">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="ae124-1115">[BREAKING CHANGE] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1115">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="ae124-1116">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1116">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="ae124-1117">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1117">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1118">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1118">Role</span></span>

* <span data-ttu-id="ae124-1119">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1119">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1120">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1120">SQL</span></span>

* <span data-ttu-id="ae124-1121">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="ae124-1121">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1122">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1122">Storage</span></span>

* <span data-ttu-id="ae124-1123">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1123">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1124">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1124">VM</span></span>

* <span data-ttu-id="ae124-1125">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="ae124-1125">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="ae124-1126">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1126">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="ae124-1127">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-1127">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ae124-1128">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1128">June 13, 2018</span></span>

<span data-ttu-id="ae124-1129">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="ae124-1129">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1130">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1130">Core</span></span>

* <span data-ttu-id="ae124-1131">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="ae124-1131">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ae124-1132">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1132">June 13, 2018</span></span>

<span data-ttu-id="ae124-1133">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ae124-1133">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ae124-1134">AKS</span><span class="sxs-lookup"><span data-stu-id="ae124-1134">AKS</span></span>

* <span data-ttu-id="ae124-1135">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1135">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ae124-1136">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1136">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="ae124-1137">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1137">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ae124-1138">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1138">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ae124-1139">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1139">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1140">AppService</span></span>

* <span data-ttu-id="ae124-1141">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1141">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ae124-1142">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1142">June 5, 2018</span></span>

<span data-ttu-id="ae124-1143">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ae124-1143">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1144">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1144">Interactive</span></span>

* <span data-ttu-id="ae124-1145">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1145">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ae124-1146">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1146">June 5, 2018</span></span>

<span data-ttu-id="ae124-1147">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ae124-1147">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1148">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1148">Core</span></span>

* <span data-ttu-id="ae124-1149">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1149">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ae124-1150">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="ae124-1150">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1151">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1151">ACR</span></span>

* <span data-ttu-id="ae124-1152">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1152">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ae124-1153">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1153">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ae124-1154">AKS</span><span class="sxs-lookup"><span data-stu-id="ae124-1154">AKS</span></span>

* <span data-ttu-id="ae124-1155">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1155">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-1156">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-1156">Batch</span></span>

* <span data-ttu-id="ae124-1157">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ae124-1157">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-1158">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-1158">IOT</span></span>

* <span data-ttu-id="ae124-1159">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1159">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1160">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1160">Network</span></span>

* <span data-ttu-id="ae124-1161">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1161">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ae124-1162">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="ae124-1162">Policy Insights</span></span>

* <span data-ttu-id="ae124-1163">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1163">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ae124-1164">ARM</span><span class="sxs-lookup"><span data-stu-id="ae124-1164">ARM</span></span>

* <span data-ttu-id="ae124-1165">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1165">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1166">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1166">SQL</span></span>

* <span data-ttu-id="ae124-1167">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1167">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ae124-1168">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1168">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ae124-1169">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1169">Storage</span></span>

* <span data-ttu-id="ae124-1170">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="ae124-1170">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1171">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1171">VM</span></span>

* <span data-ttu-id="ae124-1172">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-1172">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ae124-1173">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1173">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ae124-1174">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1174">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ae124-1175">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1175">May 22, 2018</span></span>

<span data-ttu-id="ae124-1176">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ae124-1176">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1177">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1177">Core</span></span>

* <span data-ttu-id="ae124-1178">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1178">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1179">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1179">ACS</span></span>

* <span data-ttu-id="ae124-1180">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1180">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ae124-1181">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1181">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1182">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1182">AppService</span></span>

* <span data-ttu-id="ae124-1183">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="ae124-1183">Improved generic update commands</span></span>
* <span data-ttu-id="ae124-1184">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1184">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1185">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1185">Container</span></span>

* <span data-ttu-id="ae124-1186">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1186">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ae124-1187">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1187">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1188">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1188">Extension</span></span>

* <span data-ttu-id="ae124-1189">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ae124-1189">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1190">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1190">Interactive</span></span>

* <span data-ttu-id="ae124-1191">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="ae124-1191">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ae124-1192">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="ae124-1192">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-1193">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-1193">KeyVault</span></span>

* <span data-ttu-id="ae124-1194">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="ae124-1194">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1195">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1195">Network</span></span>

* <span data-ttu-id="ae124-1196">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="ae124-1196">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ae124-1197">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="ae124-1197">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1198">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1198">SQL</span></span>

* <span data-ttu-id="ae124-1199">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="ae124-1199">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ae124-1200">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1200">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ae124-1201">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1201">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="ae124-1202">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="ae124-1202">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ae124-1203">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1203">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ae124-1204">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1204">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ae124-1205">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="ae124-1205">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ae124-1206">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1206">`edition`.</span></span> <span data-ttu-id="ae124-1207">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="ae124-1207">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ae124-1208">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1208">`elasticPoolName`.</span></span> <span data-ttu-id="ae124-1209">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="ae124-1209">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ae124-1210">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1210">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ae124-1211">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1211">`edition`.</span></span> <span data-ttu-id="ae124-1212">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1212">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ae124-1213">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1213">`dtu`.</span></span> <span data-ttu-id="ae124-1214">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1214">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ae124-1215">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1215">`databaseDtuMin`.</span></span> <span data-ttu-id="ae124-1216">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1216">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ae124-1217">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1217">`databaseDtuMax`.</span></span> <span data-ttu-id="ae124-1218">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1218">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ae124-1219">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1219">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ae124-1220">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1220">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1221">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1221">Storage</span></span>

* <span data-ttu-id="ae124-1222">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1222">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ae124-1223">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1223">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1224">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1224">VM</span></span>

* <span data-ttu-id="ae124-1225">[BREAKING CHANGE] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1225">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ae124-1226">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-1226">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ae124-1227">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1227">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ae124-1228">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1228">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ae124-1229">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1229">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ae124-1230">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1230">May 7, 2018</span></span>

<span data-ttu-id="ae124-1231">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ae124-1231">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1232">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1232">Core</span></span>

* <span data-ttu-id="ae124-1233">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="ae124-1233">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ae124-1234">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1234">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ae124-1235">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-1235">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ae124-1236">#5591</span><span class="sxs-lookup"><span data-stu-id="ae124-1236">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ae124-1237">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1237">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ae124-1238">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="ae124-1238">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ae124-1239">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="ae124-1239">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ae124-1240">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="ae124-1240">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ae124-1241">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1241">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1242">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1242">ACR</span></span>

* <span data-ttu-id="ae124-1243">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1243">Added ACR Build commands</span></span>
* <span data-ttu-id="ae124-1244">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1244">Improved resource not found error messages</span></span>
* <span data-ttu-id="ae124-1245">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="ae124-1245">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ae124-1246">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1246">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ae124-1247">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1247">Improved repository commands error messages</span></span>
* <span data-ttu-id="ae124-1248">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1248">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1249">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1249">ACS</span></span>

* <span data-ttu-id="ae124-1250">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="ae124-1250">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ae124-1251">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1251">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ae124-1252">AMS</span><span class="sxs-lookup"><span data-stu-id="ae124-1252">AMS</span></span>

* <span data-ttu-id="ae124-1253">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ae124-1253">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1254">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1254">Appservice</span></span>

* <span data-ttu-id="ae124-1255">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="ae124-1255">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ae124-1256">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1256">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ae124-1257">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1257">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ae124-1258">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1258">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ae124-1259">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-1259">Batch AI</span></span>

* <span data-ttu-id="ae124-1260">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1260">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ae124-1261">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ae124-1261">Cognitive Services</span></span>

* <span data-ttu-id="ae124-1262">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="ae124-1262">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-1263">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-1263">Consumption</span></span>

* <span data-ttu-id="ae124-1264">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1264">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1265">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1265">Container</span></span>

* <span data-ttu-id="ae124-1266">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-1266">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ae124-1267">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ae124-1267">Cosmos DB</span></span>

* <span data-ttu-id="ae124-1268">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ae124-1268">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ae124-1269">DMS</span><span class="sxs-lookup"><span data-stu-id="ae124-1269">DMS</span></span>

* <span data-ttu-id="ae124-1270">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1270">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1271">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1271">Extension</span></span>

* <span data-ttu-id="ae124-1272">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1272">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1273">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1273">Interactive</span></span>

* <span data-ttu-id="ae124-1274">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="ae124-1274">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ae124-1275">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="ae124-1275">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ae124-1276">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1276">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ae124-1277">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1277">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ae124-1278">Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-1278">Lab</span></span>

* <span data-ttu-id="ae124-1279">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1279">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1280">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1280">Network</span></span>

* <span data-ttu-id="ae124-1281">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="ae124-1281">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ae124-1282">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1282">Profile</span></span>

* <span data-ttu-id="ae124-1283">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1283">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ae124-1284">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1284">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ae124-1285">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1285">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ae124-1286">Redis</span><span class="sxs-lookup"><span data-stu-id="ae124-1286">Redis</span></span>

* <span data-ttu-id="ae124-1287">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1287">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ae124-1288">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1288">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ae124-1289">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1289">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ae124-1290">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1290">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ae124-1291">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1291">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1292">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1292">Role</span></span>

* <span data-ttu-id="ae124-1293">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1293">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1294">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1294">Storage</span></span>

* <span data-ttu-id="ae124-1295">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1295">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ae124-1296">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="ae124-1296">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ae124-1297">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="ae124-1297">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ae124-1298">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="ae124-1298">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ae124-1299">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ae124-1299">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1300">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1300">VM</span></span>

* <span data-ttu-id="ae124-1301">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1301">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ae124-1302">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1302">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ae124-1303">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="ae124-1303">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ae124-1304">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1304">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ae124-1305">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="ae124-1305">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ae124-1306">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1306">Added write accelerator support</span></span>
* <span data-ttu-id="ae124-1307">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1307">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ae124-1308">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="ae124-1308">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ae124-1309">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="ae124-1309">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ae124-1310">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1310">April 10, 2018</span></span>

<span data-ttu-id="ae124-1311">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ae124-1311">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1312">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1312">ACR</span></span>

* <span data-ttu-id="ae124-1313">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="ae124-1313">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1314">ACS</span></span>

* <span data-ttu-id="ae124-1315">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1315">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1316">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1316">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ae124-1318">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1318">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ae124-1319">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ae124-1319">BatchAI</span></span>

* <span data-ttu-id="ae124-1320">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1320">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="ae124-1321">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="ae124-1321">Job level mounting</span></span>
  - <span data-ttu-id="ae124-1322">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="ae124-1322">Environment variables with secret values</span></span>
  - <span data-ttu-id="ae124-1323">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="ae124-1323">Performance counters settings</span></span>
  - <span data-ttu-id="ae124-1324">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="ae124-1324">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="ae124-1325">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="ae124-1325">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="ae124-1326">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="ae124-1326">Usage and limits reporting</span></span>
  - <span data-ttu-id="ae124-1327">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="ae124-1327">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="ae124-1328">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="ae124-1328">Support for custom images</span></span>
  - <span data-ttu-id="ae124-1329">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1329">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ae124-1330">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="ae124-1330">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ae124-1331">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1331">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ae124-1332">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae124-1332">National clouds are supported</span></span>
* <span data-ttu-id="ae124-1333">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1333">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ae124-1334">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="ae124-1334">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ae124-1335">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1335">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ae124-1336">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="ae124-1336">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ae124-1337">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="ae124-1337">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ae124-1338">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="ae124-1338">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ae124-1339">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="ae124-1339">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ae124-1340">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1340">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ae124-1341">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="ae124-1341">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ae124-1342">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1342">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ae124-1343">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="ae124-1343">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ae124-1344">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1344">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ae124-1345">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="ae124-1345">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ae124-1346">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="ae124-1346">Billing</span></span>

* <span data-ttu-id="ae124-1347">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1347">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-1348">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-1348">Consumption</span></span>

* <span data-ttu-id="ae124-1349">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1349">Added `marketplace` commands</span></span>
* <span data-ttu-id="ae124-1350">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1350">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ae124-1351">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1351">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ae124-1352">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1352">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ae124-1353">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1353">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ae124-1354">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1354">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1355">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1355">Container</span></span>

* <span data-ttu-id="ae124-1356">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1356">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ae124-1357">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-1357">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1358">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1358">Extension</span></span>

* <span data-ttu-id="ae124-1359">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1359">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1360">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1360">Interactive</span></span>

* <span data-ttu-id="ae124-1361">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="ae124-1361">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ae124-1362">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1362">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ae124-1363">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1363">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1364">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1364">Network</span></span>

* <span data-ttu-id="ae124-1365">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-1365">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ae124-1366">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1366">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="ae124-1367">#4910</span><span class="sxs-lookup"><span data-stu-id="ae124-1367">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="ae124-1368">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1368">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="ae124-1369">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1369">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ae124-1370">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1370">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ae124-1371">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1371">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ae124-1372">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1372">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1373">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1373">Profile</span></span>

* <span data-ttu-id="ae124-1374">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1374">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ae124-1375">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1375">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-1376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-1376">RDBMS</span></span>

* <span data-ttu-id="ae124-1377">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1377">Added `georestore` command</span></span>
* <span data-ttu-id="ae124-1378">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1378">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1379">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1379">Resource</span></span>

* <span data-ttu-id="ae124-1380">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1380">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ae124-1381">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1381">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1382">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1382">SQL</span></span>

* <span data-ttu-id="ae124-1383">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1383">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1384">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1384">Storage</span></span>

* <span data-ttu-id="ae124-1385">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1385">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1386">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1386">VM</span></span>

* <span data-ttu-id="ae124-1387">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1387">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ae124-1388">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1388">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="ae124-1390">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1390">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ae124-1391">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="ae124-1391">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="ae124-1392">#5718</span><span class="sxs-lookup"><span data-stu-id="ae124-1392">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="ae124-1393">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="ae124-1393">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ae124-1394">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1394">March 27, 2018</span></span>

<span data-ttu-id="ae124-1395">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ae124-1395">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1396">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1396">Core</span></span>

* <span data-ttu-id="ae124-1397">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="ae124-1397">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1398">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1398">ACS</span></span>

* <span data-ttu-id="ae124-1399">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="ae124-1399">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1400">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1400">Appservice</span></span>

* <span data-ttu-id="ae124-1401">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1401">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ae124-1402">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1402">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ae124-1403">Backup</span><span class="sxs-lookup"><span data-stu-id="ae124-1403">Backup</span></span>

* <span data-ttu-id="ae124-1404">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1404">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ae124-1405">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="ae124-1405">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ae124-1406">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="ae124-1406">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="ae124-1407">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="ae124-1407">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1408">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1408">Container</span></span>

* <span data-ttu-id="ae124-1409">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1409">Added `container exec` command.</span></span> <span data-ttu-id="ae124-1410">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="ae124-1410">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ae124-1411">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="ae124-1411">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1412">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1412">Extension</span></span>

* <span data-ttu-id="ae124-1413">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="ae124-1413">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ae124-1414">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-1414">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ae124-1415">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-1415">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1416">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1416">Interactive</span></span>

* <span data-ttu-id="ae124-1417">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-1417">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ae124-1418">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1418">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ae124-1419">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="ae124-1419">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ae124-1420">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="ae124-1420">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ae124-1421">Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-1421">Lab</span></span>

* <span data-ttu-id="ae124-1422">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1422">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1423">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1423">Monitor</span></span>

* <span data-ttu-id="ae124-1424">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="ae124-1424">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ae124-1425">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="ae124-1425">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ae124-1426">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="ae124-1426">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1427">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1427">Network</span></span>

* <span data-ttu-id="ae124-1428">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1428">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1429">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1429">Profile</span></span>

* <span data-ttu-id="ae124-1430">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1430">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-1431">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-1431">RDBMS</span></span>

* <span data-ttu-id="ae124-1432">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1432">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1433">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1433">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ae124-1435">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1435">Role</span></span>

* <span data-ttu-id="ae124-1436">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1436">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ae124-1437">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="ae124-1437">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ae124-1438">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1438">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ae124-1439">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1439">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ae124-1440">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1440">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1441">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1441">Storage</span></span>

* <span data-ttu-id="ae124-1442">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1442">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ae124-1443">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="ae124-1443">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1444">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1444">VM</span></span>

* <span data-ttu-id="ae124-1445">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1445">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ae124-1446">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1446">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ae124-1447">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="ae124-1447">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ae124-1448">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="ae124-1448">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ae124-1449">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1449">March 13, 2018</span></span>

<span data-ttu-id="ae124-1450">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ae124-1450">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1451">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1451">ACR</span></span>

* <span data-ttu-id="ae124-1452">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1452">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ae124-1453">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1453">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ae124-1454">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1454">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1455">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1455">ACS</span></span>

* <span data-ttu-id="ae124-1456">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1456">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ae124-1457">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1457">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ae124-1458">Advisor</span><span class="sxs-lookup"><span data-stu-id="ae124-1458">Advisor</span></span>

* <span data-ttu-id="ae124-1459">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1459">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ae124-1460">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1460">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ae124-1461">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1461">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="ae124-1462">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1462">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ae124-1463">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1463">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1464">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1464">Appservice</span></span>

* <span data-ttu-id="ae124-1465">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1465">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ae124-1466">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1466">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ae124-1467">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="ae124-1467">Eventhubs</span></span>

* <span data-ttu-id="ae124-1468">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1468">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1469">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1469">Extension</span></span>

* <span data-ttu-id="ae124-1470">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="ae124-1470">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1471">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1471">Interactive</span></span>

* <span data-ttu-id="ae124-1472">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="ae124-1472">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ae124-1473">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="ae124-1473">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ae124-1474">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="ae124-1474">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ae124-1475">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1475">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1476">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1476">Monitor</span></span>

* <span data-ttu-id="ae124-1477">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1477">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ae124-1478">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1478">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ae124-1479">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1479">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ae124-1480">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1480">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1481">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1481">Network</span></span>

* <span data-ttu-id="ae124-1482">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1482">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ae124-1483">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1483">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ae124-1484">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1484">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ae124-1485">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1485">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1486">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1486">Profile</span></span>

* <span data-ttu-id="ae124-1487">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1487">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ae124-1488">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1488">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-1489">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-1489">RDBMS</span></span>

* <span data-ttu-id="ae124-1490">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1490">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ae124-1491">Service Bus</span><span class="sxs-lookup"><span data-stu-id="ae124-1491">Service Bus</span></span>

* <span data-ttu-id="ae124-1492">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1492">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1493">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1493">Storage</span></span>

* <span data-ttu-id="ae124-1494">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="ae124-1494">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ae124-1495">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="ae124-1495">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1496">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1496">VM</span></span>

* <span data-ttu-id="ae124-1497">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="ae124-1497">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ae124-1498">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1498">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ae124-1499">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1499">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ae124-1500">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1500">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ae124-1501">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1501">February 27, 2018</span></span>

<span data-ttu-id="ae124-1502">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ae124-1502">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1503">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1503">Core</span></span>

* <span data-ttu-id="ae124-1504">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="ae124-1504">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ae124-1505">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1505">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ae124-1506">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1506">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1507">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1507">ACS</span></span>

* <span data-ttu-id="ae124-1508">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1508">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ae124-1509">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="ae124-1509">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ae124-1510">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1510">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ae124-1511">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1511">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1512">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1512">Appservice</span></span>

* <span data-ttu-id="ae124-1513">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ae124-1513">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ae124-1514">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="ae124-1514">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ae124-1515">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ae124-1515">Cognitive Services</span></span>

* <span data-ttu-id="ae124-1516">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1516">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-1517">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-1517">Consumption</span></span>

* <span data-ttu-id="ae124-1518">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1518">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ae124-1519">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1519">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1520">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1520">Container</span></span>

* <span data-ttu-id="ae124-1521">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="ae124-1521">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1522">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1522">Network</span></span>

* <span data-ttu-id="ae124-1523">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="ae124-1523">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1524">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1524">Resource</span></span>

* <span data-ttu-id="ae124-1525">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="ae124-1525">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1526">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1526">Role</span></span>

* <span data-ttu-id="ae124-1527">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1527">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1528">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1528">SQL</span></span>

* <span data-ttu-id="ae124-1529">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="ae124-1529">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1530">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1530">Storage</span></span>

* <span data-ttu-id="ae124-1531">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-1531">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1532">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1532">VM</span></span>

* <span data-ttu-id="ae124-1533">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1533">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ae124-1534">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1534">February 13, 2018</span></span>

<span data-ttu-id="ae124-1535">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ae124-1535">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1536">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1536">Core</span></span>

* <span data-ttu-id="ae124-1537">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1537">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1538">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1538">ACS</span></span>

* <span data-ttu-id="ae124-1539">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1539">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ae124-1540">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1540">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ae124-1541">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1541">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ae124-1542">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1542">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ae124-1543">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1543">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ae124-1544">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1544">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ae124-1545">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="ae124-1545">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ae124-1546">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="ae124-1546">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1547">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1547">Appservice</span></span>

* <span data-ttu-id="ae124-1548">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="ae124-1548">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ae124-1549">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1549">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-1550">CDN</span></span>

* <span data-ttu-id="ae124-1551">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1551">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1552">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1552">Container</span></span>

* <span data-ttu-id="ae124-1553">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1553">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ae124-1554">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1554">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-1555">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-1555">CosmosDB</span></span>

* <span data-ttu-id="ae124-1556">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1556">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1557">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1557">Extension</span></span>

* <span data-ttu-id="ae124-1558">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1558">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ae124-1559">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1559">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ae124-1560">Feedback</span><span class="sxs-lookup"><span data-stu-id="ae124-1560">Feedback</span></span>

* <span data-ttu-id="ae124-1561">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1561">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1562">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1562">Interactive</span></span>

* <span data-ttu-id="ae124-1563">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1563">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ae124-1564">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1564">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-1565">IoT</span></span>

* <span data-ttu-id="ae124-1566">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="ae124-1566">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ae124-1567">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="ae124-1567">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ae124-1568">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1568">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ae124-1569">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1569">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1570">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1570">Monitor</span></span>

* <span data-ttu-id="ae124-1571">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1571">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1572">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1572">Network</span></span>

* <span data-ttu-id="ae124-1573">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="ae124-1573">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ae124-1574">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1574">Profile</span></span>

* <span data-ttu-id="ae124-1575">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="ae124-1575">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1576">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1576">Resource</span></span>

* <span data-ttu-id="ae124-1577">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1577">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1578">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1578">Role</span></span>

* <span data-ttu-id="ae124-1579">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1579">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1580">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1580">SQL</span></span>

* <span data-ttu-id="ae124-1581">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1581">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ae124-1582">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1582">Added `sql db rename`</span></span>
* <span data-ttu-id="ae124-1583">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1583">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1584">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1584">Storage</span></span>

* <span data-ttu-id="ae124-1585">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1585">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1586">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1586">VM</span></span>

* <span data-ttu-id="ae124-1587">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1587">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ae124-1588">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1588">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ae124-1589">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="ae124-1589">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ae124-1590">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1590">January 31, 2018</span></span>

<span data-ttu-id="ae124-1591">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ae124-1591">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1592">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1592">Core</span></span>

* <span data-ttu-id="ae124-1593">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1593">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ae124-1594">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1594">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ae124-1595">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="ae124-1595">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ae124-1596">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="ae124-1596">Use `--verbose` to see</span></span>
* <span data-ttu-id="ae124-1597">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1597">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1598">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1598">ACS</span></span>

* <span data-ttu-id="ae124-1599">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="ae124-1599">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ae124-1600">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1600">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1601">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1601">Appservice</span></span>

* <span data-ttu-id="ae124-1602">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="ae124-1602">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ae124-1603">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1603">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-1604">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-1604">CDN</span></span>

* <span data-ttu-id="ae124-1605">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1605">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-1606">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-1606">CosmosDB</span></span>

* <span data-ttu-id="ae124-1607">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1607">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1608">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1608">Interactive</span></span>

* <span data-ttu-id="ae124-1609">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1609">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1610">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1610">Network</span></span>

* <span data-ttu-id="ae124-1611">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1611">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ae124-1612">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="ae124-1612">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ae124-1613">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1613">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ae124-1614">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1614">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ae124-1615">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1615">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ae124-1616">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="ae124-1616">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ae124-1617">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1617">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ae124-1618">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1618">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ae124-1619">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1619">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="ae124-1620">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="ae124-1620">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1621">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1621">Profile</span></span>

* <span data-ttu-id="ae124-1622">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1622">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1623">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1623">Resource</span></span>

* <span data-ttu-id="ae124-1624">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="ae124-1624">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1625">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1625">Storage</span></span>

* <span data-ttu-id="ae124-1626">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1626">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ae124-1627">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1627">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ae124-1628">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="ae124-1628">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="ae124-1629">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1629">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ae124-1630">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="ae124-1630">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1631">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1631">VM</span></span>

* <span data-ttu-id="ae124-1632">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1632">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ae124-1633">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="ae124-1633">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ae124-1634">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1634">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ae124-1635">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1635">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ae124-1636">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="ae124-1636">January 17, 2018</span></span>

<span data-ttu-id="ae124-1637">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ae124-1637">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1638">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1638">ACR</span></span>

* <span data-ttu-id="ae124-1639">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1639">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ae124-1640">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="ae124-1640">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1641">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1641">ACS</span></span>

* <span data-ttu-id="ae124-1642">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1642">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ae124-1643">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1643">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1644">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1644">Appservice</span></span>

* <span data-ttu-id="ae124-1645">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="ae124-1645">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ae124-1646">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1646">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ae124-1647">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1647">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ae124-1648">Backup</span><span class="sxs-lookup"><span data-stu-id="ae124-1648">Backup</span></span>

* <span data-ttu-id="ae124-1649">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="ae124-1649">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ae124-1650">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1650">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ae124-1651">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="ae124-1651">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ae124-1652">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="ae124-1652">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ae124-1653">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="ae124-1653">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-1654">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-1654">Batch</span></span>

* <span data-ttu-id="ae124-1655">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="ae124-1655">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ae124-1656">Cloud</span><span class="sxs-lookup"><span data-stu-id="ae124-1656">Cloud</span></span>

* <span data-ttu-id="ae124-1657">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1657">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-1658">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-1658">Consumption</span></span>

* <span data-ttu-id="ae124-1659">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="ae124-1659">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ae124-1660">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ae124-1660">Event Grid</span></span>

* <span data-ttu-id="ae124-1661">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-1661">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ae124-1662">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-1662">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ae124-1663">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1663">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ae124-1664">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1664">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ae124-1665">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1665">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ae124-1666">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1666">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ae124-1667">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1667">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ae124-1668">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1668">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-1669">Interactive</span><span class="sxs-lookup"><span data-stu-id="ae124-1669">Interactive</span></span>

* <span data-ttu-id="ae124-1670">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-1670">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ae124-1671">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1671">Fixed errors on startup</span></span>
* <span data-ttu-id="ae124-1672">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-1672">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-1673">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-1673">IoT</span></span>

* <span data-ttu-id="ae124-1674">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1674">Added support for device provisioning service</span></span>
* <span data-ttu-id="ae124-1675">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1675">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ae124-1676">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="ae124-1676">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1677">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1677">Monitor</span></span>

* <span data-ttu-id="ae124-1678">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1678">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ae124-1679">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae124-1679">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ae124-1680">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1680">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1681">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1681">Network</span></span>

* <span data-ttu-id="ae124-1682">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="ae124-1682">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ae124-1683">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1683">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1684">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1684">Profile</span></span>

* <span data-ttu-id="ae124-1685">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1685">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1686">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1686">Role</span></span>

* <span data-ttu-id="ae124-1687">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="ae124-1687">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ae124-1688">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ae124-1688">Service Fabric</span></span>

* <span data-ttu-id="ae124-1689">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1689">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ae124-1690">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1690">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1691">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1691">VM</span></span>

* <span data-ttu-id="ae124-1692">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="ae124-1692">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ae124-1693">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1693">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ae124-1694">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="ae124-1694">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ae124-1695">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1695">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ae124-1696">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1696">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ae124-1697">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1697">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ae124-1698">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1698">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ae124-1699">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1699">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ae124-1700">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1700">December 19, 2017</span></span>

<span data-ttu-id="ae124-1701">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ae124-1701">Version 2.0.23</span></span>

* <span data-ttu-id="ae124-1702">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1702">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1703">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1703">Container</span></span>

* <span data-ttu-id="ae124-1704">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1704">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1705">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1705">Network</span></span>

* <span data-ttu-id="ae124-1706">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1706">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ae124-1707">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1707">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1708">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1708">Storage</span></span>

* <span data-ttu-id="ae124-1709">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1709">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1710">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1710">VM</span></span>

* <span data-ttu-id="ae124-1711">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1711">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ae124-1712">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1712">December 5, 2017</span></span>

<span data-ttu-id="ae124-1713">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ae124-1713">Version 2.0.22</span></span>

* <span data-ttu-id="ae124-1714">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1714">Removed `az component` commands.</span></span> <span data-ttu-id="ae124-1715">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1715">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1716">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1716">Core</span></span>
* <span data-ttu-id="ae124-1717">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1717">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ae124-1718">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1718">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1719">ACS</span></span>

* <span data-ttu-id="ae124-1720">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1720">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ae124-1721">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="ae124-1721">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ae124-1722">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="ae124-1722">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ae124-1723">Advisor</span><span class="sxs-lookup"><span data-stu-id="ae124-1723">Advisor</span></span>

* <span data-ttu-id="ae124-1724">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1724">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1725">Appservice</span></span>

* <span data-ttu-id="ae124-1726">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="ae124-1726">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ae124-1727">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ae124-1727">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ae124-1728">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1728">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ae124-1729">Nutzung</span><span class="sxs-lookup"><span data-stu-id="ae124-1729">Consumption</span></span>

* <span data-ttu-id="ae124-1730">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1730">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1731">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1731">Container</span></span>

* <span data-ttu-id="ae124-1732">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="ae124-1732">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1733">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1733">Monitor</span></span>

* <span data-ttu-id="ae124-1734">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1734">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1735">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1735">Resource</span></span>

* <span data-ttu-id="ae124-1736">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1736">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ae124-1737">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-1737">Role</span></span>

* <span data-ttu-id="ae124-1738">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1738">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ae124-1739">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1739">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ae124-1740">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="ae124-1740">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1741">SQL</span></span>

* <span data-ttu-id="ae124-1742">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1742">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ae124-1743">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1743">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1744">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1744">VM</span></span>

* <span data-ttu-id="ae124-1745">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1745">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ae124-1746">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1746">November 14, 2017</span></span>

<span data-ttu-id="ae124-1747">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ae124-1747">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1748">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1748">ACR</span></span>

* <span data-ttu-id="ae124-1749">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1749">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ae124-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1750">ACS</span></span>

* <span data-ttu-id="ae124-1751">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1751">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ae124-1752">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="ae124-1752">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ae124-1753">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="ae124-1753">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ae124-1754">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1754">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ae124-1755">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1755">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1756">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1756">Appservice</span></span>

* <span data-ttu-id="ae124-1757">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1757">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ae124-1758">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1758">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ae124-1759">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1759">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ae124-1760">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-1760">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ae124-1761">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1761">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ae124-1762">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="ae124-1762">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-1763">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-1763">Batch</span></span>

* <span data-ttu-id="ae124-1764">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="ae124-1764">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ae124-1765">BatchAI</span><span class="sxs-lookup"><span data-stu-id="ae124-1765">Batchai</span></span>

* <span data-ttu-id="ae124-1766">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1766">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ae124-1767">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1767">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ae124-1768">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1768">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ae124-1769">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1769">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ae124-1770">Cloud</span><span class="sxs-lookup"><span data-stu-id="ae124-1770">Cloud</span></span>

* <span data-ttu-id="ae124-1771">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="ae124-1771">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ae124-1772">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-1772">Container</span></span>

* <span data-ttu-id="ae124-1773">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1773">Added support to open multiple ports</span></span>
* <span data-ttu-id="ae124-1774">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1774">Added container group restart policy</span></span>
* <span data-ttu-id="ae124-1775">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1775">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ae124-1776">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1776">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ae124-1777">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ae124-1777">Data Lake Analytics</span></span>

* <span data-ttu-id="ae124-1778">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="ae124-1778">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ae124-1779">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ae124-1779">Data Lake Store</span></span>

* <span data-ttu-id="ae124-1780">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="ae124-1780">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1781">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1781">Extension</span></span>

* <span data-ttu-id="ae124-1782">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1782">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ae124-1783">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="ae124-1783">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-1784">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-1784">IoT</span></span>

* <span data-ttu-id="ae124-1785">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1785">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1786">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1786">Monitor</span></span>

* <span data-ttu-id="ae124-1787">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1787">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1788">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1788">Network</span></span>

* <span data-ttu-id="ae124-1789">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1789">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ae124-1790">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-1790">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ae124-1791">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="ae124-1791">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ae124-1792">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1792">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ae124-1793">Reservations</span><span class="sxs-lookup"><span data-stu-id="ae124-1793">Reservations</span></span>

* <span data-ttu-id="ae124-1794">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="ae124-1794">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1795">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1795">Resource</span></span>

* <span data-ttu-id="ae124-1796">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1796">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1797">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1797">SQL</span></span>

* <span data-ttu-id="ae124-1798">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1798">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1799">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1799">Storage</span></span>

* <span data-ttu-id="ae124-1800">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1800">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ae124-1801">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="ae124-1801">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ae124-1802">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="ae124-1802">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ae124-1803">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1803">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ae124-1804">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1804">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ae124-1805">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1805">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ae124-1806">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1806">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1807">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1807">VM</span></span>

* <span data-ttu-id="ae124-1808">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="ae124-1808">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ae124-1809">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1809">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ae124-1810">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="ae124-1810">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ae124-1811">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1811">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ae124-1812">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1812">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ae124-1813">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1813">October 24, 2017</span></span>

<span data-ttu-id="ae124-1814">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ae124-1814">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1815">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1815">Core</span></span>

* <span data-ttu-id="ae124-1816">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="ae124-1816">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-1817">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-1817">ACR</span></span>

* <span data-ttu-id="ae124-1818">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="ae124-1818">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ae124-1819">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1819">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ae124-1820">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1820">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1821">ACS</span></span>

* <span data-ttu-id="ae124-1822">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1822">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ae124-1823">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1823">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1824">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1824">Appservice</span></span>

* <span data-ttu-id="ae124-1825">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="ae124-1825">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ae124-1826">Komponente</span><span class="sxs-lookup"><span data-stu-id="ae124-1826">Component</span></span>

* <span data-ttu-id="ae124-1827">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1827">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-1828">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-1828">Monitor</span></span>

* <span data-ttu-id="ae124-1829">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1829">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1830">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1830">Resource</span></span>

* <span data-ttu-id="ae124-1831">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1831">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ae124-1832">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="ae124-1832">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1833">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1833">VM</span></span>

* <span data-ttu-id="ae124-1834">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1834">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ae124-1835">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1835">October 9, 2017</span></span>

<span data-ttu-id="ae124-1836">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ae124-1836">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1837">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1837">Core</span></span>

* <span data-ttu-id="ae124-1838">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1838">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1839">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1839">Appservice</span></span>

* <span data-ttu-id="ae124-1840">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1840">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-1841">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-1841">Batch</span></span>

* <span data-ttu-id="ae124-1842">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ae124-1842">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ae124-1843">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1843">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ae124-1844">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1844">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ae124-1845">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1845">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ae124-1846">BatchAI</span><span class="sxs-lookup"><span data-stu-id="ae124-1846">Batchai</span></span>

* <span data-ttu-id="ae124-1847">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-1847">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-1848">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-1848">Keyvault</span></span>

* <span data-ttu-id="ae124-1849">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="ae124-1849">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ae124-1850">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ae124-1850">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ae124-1851">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1851">Network</span></span>

* <span data-ttu-id="ae124-1852">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="ae124-1852">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ae124-1853">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1853">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1854">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1854">Resource</span></span>

* <span data-ttu-id="ae124-1855">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1855">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ae124-1856">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1856">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ae124-1857">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1857">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ae124-1858">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1858">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1859">Sql</span><span class="sxs-lookup"><span data-stu-id="ae124-1859">Sql</span></span>

* <span data-ttu-id="ae124-1860">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1860">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ae124-1861">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1861">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ae124-1862">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1862">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1863">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1863">Storage</span></span>

* <span data-ttu-id="ae124-1864">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1864">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1865">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1865">Vm</span></span>

* <span data-ttu-id="ae124-1866">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="ae124-1866">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ae124-1867">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1867">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ae124-1868">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1868">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ae124-1869">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1869">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ae124-1870">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1870">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ae124-1871">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1871">September 22, 2017</span></span>

<span data-ttu-id="ae124-1872">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ae124-1872">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1873">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1873">Resource</span></span>

* <span data-ttu-id="ae124-1874">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1874">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ae124-1875">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1875">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ae124-1876">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1876">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ae124-1877">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="ae124-1877">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1878">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1878">Network</span></span>

* <span data-ttu-id="ae124-1879">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1879">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ae124-1880">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1880">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ae124-1881">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1881">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ae124-1882">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1882">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ae124-1883">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1883">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ae124-1884">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1884">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ae124-1885">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1885">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1886">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1886">Storage</span></span>

* <span data-ttu-id="ae124-1887">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="ae124-1887">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ae124-1888">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="ae124-1888">Eventgrid</span></span>

* <span data-ttu-id="ae124-1889">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1889">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1890">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1890">SQL</span></span>

* <span data-ttu-id="ae124-1891">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="ae124-1891">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ae124-1892">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae124-1892">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ae124-1893">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1893">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-1894">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-1894">Keyvault</span></span>

* <span data-ttu-id="ae124-1895">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1895">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1896">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1896">VM</span></span>

* <span data-ttu-id="ae124-1897">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1897">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ae124-1898">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="ae124-1898">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ae124-1899">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1899">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ae124-1900">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1900">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ae124-1901">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1901">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ae124-1902">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1902">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1903">ACS</span></span>

* <span data-ttu-id="ae124-1904">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1904">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1905">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1905">Appservice</span></span>

* <span data-ttu-id="ae124-1906">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ae124-1906">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ae124-1907">Backup</span><span class="sxs-lookup"><span data-stu-id="ae124-1907">Backup</span></span>

* <span data-ttu-id="ae124-1908">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="ae124-1908">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ae124-1909">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1909">September 11, 2017</span></span>

<span data-ttu-id="ae124-1910">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ae124-1910">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ae124-1911">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-1911">Core</span></span>

* <span data-ttu-id="ae124-1912">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="ae124-1912">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ae124-1913">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="ae124-1913">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1914">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1914">Acs</span></span>

* <span data-ttu-id="ae124-1915">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1915">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ae124-1916">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="ae124-1916">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1917">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1917">Appservice</span></span>

* <span data-ttu-id="ae124-1918">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="ae124-1918">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-1919">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-1919">CDN</span></span>

* <span data-ttu-id="ae124-1920">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="ae124-1920">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ae124-1921">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="ae124-1921">Extension</span></span>

* <span data-ttu-id="ae124-1922">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1922">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-1923">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-1923">Keyvault</span></span>

* <span data-ttu-id="ae124-1924">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="ae124-1924">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1925">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1925">Network</span></span>

* <span data-ttu-id="ae124-1926">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1926">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ae124-1927">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1927">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ae124-1928">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1928">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ae124-1929">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1929">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ae124-1930">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1930">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-1931">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-1931">Resource</span></span>

* <span data-ttu-id="ae124-1932">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="ae124-1932">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ae124-1933">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="ae124-1933">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ae124-1934">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="ae124-1934">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ae124-1935">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="ae124-1935">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-1936">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-1936">SQL</span></span>

* <span data-ttu-id="ae124-1937">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1937">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1938">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1938">VM</span></span>

* <span data-ttu-id="ae124-1939">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="ae124-1939">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ae124-1940">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="ae124-1940">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ae124-1941">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1941">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ae124-1942">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="ae124-1942">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ae124-1943">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="ae124-1943">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ae124-1944">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1944">August 31, 2017</span></span>

<span data-ttu-id="ae124-1945">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ae124-1945">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-1946">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-1946">Keyvault</span></span>

* <span data-ttu-id="ae124-1947">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="ae124-1947">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ae124-1948">Sf</span><span class="sxs-lookup"><span data-stu-id="ae124-1948">Sf</span></span>

* <span data-ttu-id="ae124-1949">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ae124-1949">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1950">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1950">Storage</span></span>

* <span data-ttu-id="ae124-1951">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="ae124-1951">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ae124-1952">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="ae124-1952">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ae124-1953">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1953">August 28, 2017</span></span>

<span data-ttu-id="ae124-1954">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ae124-1954">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ae124-1955">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="ae124-1955">CLI</span></span>

* <span data-ttu-id="ae124-1956">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1956">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1957">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1957">ACS</span></span>

* <span data-ttu-id="ae124-1958">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1958">Corrected preview regions</span></span>
* <span data-ttu-id="ae124-1959">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1959">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ae124-1960">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1960">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-1961">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-1961">Appservice</span></span>

* <span data-ttu-id="ae124-1962">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1962">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ae124-1963">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1963">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ae124-1964">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-1964">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ae124-1965">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="ae124-1965">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ae124-1966">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="ae124-1966">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-1967">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-1967">IoT</span></span>

* <span data-ttu-id="ae124-1968">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="ae124-1968">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ae124-1969">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-1969">Network</span></span>

* <span data-ttu-id="ae124-1970">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1970">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ae124-1971">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1971">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ae124-1972">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1972">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ae124-1973">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1973">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ae124-1974">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1974">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-1975">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-1975">Profile</span></span>

* <span data-ttu-id="ae124-1976">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-1976">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ae124-1977">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ae124-1977">Service Fabric</span></span>

* <span data-ttu-id="ae124-1978">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="ae124-1978">Preview release</span></span>
* <span data-ttu-id="ae124-1979">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="ae124-1979">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ae124-1980">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1980">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ae124-1981">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1981">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-1982">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-1982">Storage</span></span>

* <span data-ttu-id="ae124-1983">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-1983">Enabled setting blob tier</span></span>
* <span data-ttu-id="ae124-1984">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1984">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ae124-1985">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-1985">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ae124-1986">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-1986">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ae124-1987">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-1987">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ae124-1988">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="ae124-1988">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-1989">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-1989">VM</span></span>

* <span data-ttu-id="ae124-1990">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-1990">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ae124-1991">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-1991">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ae124-1992">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-1992">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ae124-1993">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-1993">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ae124-1994">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-1994">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ae124-1995">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-1995">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ae124-1996">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-1996">August 15, 2017</span></span>

<span data-ttu-id="ae124-1997">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ae124-1997">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-1998">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-1998">ACS</span></span>

* <span data-ttu-id="ae124-1999">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-1999">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-2000">Appservice</span></span>

* <span data-ttu-id="ae124-2001">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-2001">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ae124-2002">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ae124-2002">Event Grid</span></span>

* <span data-ttu-id="ae124-2003">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2003">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ae124-2004">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-2004">August 11, 2017</span></span>

<span data-ttu-id="ae124-2005">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ae124-2005">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-2006">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-2006">ACS</span></span>

* <span data-ttu-id="ae124-2007">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2007">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-2008">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-2008">Batch</span></span>

* <span data-ttu-id="ae124-2009">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-2009">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ae124-2010">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2010">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ae124-2011">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-2011">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ae124-2012">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="ae124-2012">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ae124-2013">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="ae124-2013">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ae124-2014">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2014">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ae124-2015">Komponente</span><span class="sxs-lookup"><span data-stu-id="ae124-2015">Component</span></span>

* <span data-ttu-id="ae124-2016">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2016">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ae124-2017">Container</span><span class="sxs-lookup"><span data-stu-id="ae124-2017">Container</span></span>

* <span data-ttu-id="ae124-2018">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="ae124-2018">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ae124-2019">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ae124-2019">Data Lake Store</span></span>

* <span data-ttu-id="ae124-2020">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-2020">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ae124-2021">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ae124-2021">Event Grid</span></span>

* <span data-ttu-id="ae124-2022">Erste Version</span><span class="sxs-lookup"><span data-stu-id="ae124-2022">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ae124-2023">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-2023">Network</span></span>

* <span data-ttu-id="ae124-2024">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-2024">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ae124-2025">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-2025">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ae124-2026">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-2026">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ae124-2027">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="ae124-2027">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-2028">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-2028">Profile</span></span>

* <span data-ttu-id="ae124-2029">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="ae124-2029">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-2030">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-2030">Storage</span></span>

* <span data-ttu-id="ae124-2031">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-2031">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-2032">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-2032">VM</span></span>

* <span data-ttu-id="ae124-2033">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-2033">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ae124-2034">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-2034">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ae124-2035">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="ae124-2035">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ae124-2036">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="ae124-2036">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ae124-2037">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-2037">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ae124-2038">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-2038">July 28, 2017</span></span>

<span data-ttu-id="ae124-2039">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ae124-2039">Version 2.0.12</span></span>

* <span data-ttu-id="ae124-2040">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2040">Added container commands</span></span>
* <span data-ttu-id="ae124-2041">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2041">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ae124-2042">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-2042">Core</span></span>

* <span data-ttu-id="ae124-2043">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="ae124-2043">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ae124-2044">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-2044">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ae124-2045">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="ae124-2045">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ae124-2046">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="ae124-2046">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ae124-2047">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="ae124-2047">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ae124-2048">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="ae124-2048">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ae124-2049">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="ae124-2049">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ae124-2050">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="ae124-2050">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ae124-2051">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="ae124-2051">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ae124-2052">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-2052">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ae124-2053">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="ae124-2053">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ae124-2054">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="ae124-2054">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ae124-2055">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="ae124-2055">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ae124-2056">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="ae124-2056">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ae124-2057">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="ae124-2057">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ae124-2058">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="ae124-2058">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ae124-2059">ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-2059">ACR</span></span>

* <span data-ttu-id="ae124-2060">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2060">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ae124-2061">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="ae124-2061">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ae124-2062">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2062">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ae124-2063">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2063">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ae124-2064">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2064">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ae124-2065">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2065">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-2066">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-2066">ACS</span></span>

* <span data-ttu-id="ae124-2067">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="ae124-2067">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-2068">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-2068">Appservice</span></span>

* <span data-ttu-id="ae124-2069">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="ae124-2069">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ae124-2070">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="ae124-2070">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ae124-2071">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="ae124-2071">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ae124-2072">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="ae124-2072">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ae124-2073">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="ae124-2073">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ae124-2074">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="ae124-2074">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ae124-2075">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="ae124-2075">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ae124-2076">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="ae124-2076">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ae124-2077">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="ae124-2077">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ae124-2078">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ae124-2078">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ae124-2079">Batch</span><span class="sxs-lookup"><span data-stu-id="ae124-2079">Batch</span></span>

* <span data-ttu-id="ae124-2080">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-2080">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ae124-2081">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-2081">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ae124-2082">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2082">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ae124-2083">CDN</span><span class="sxs-lookup"><span data-stu-id="ae124-2083">CDN</span></span>

* <span data-ttu-id="ae124-2084">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="ae124-2084">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ae124-2085">Cloud</span><span class="sxs-lookup"><span data-stu-id="ae124-2085">Cloud</span></span>

* <span data-ttu-id="ae124-2086">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="ae124-2086">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ae124-2087">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae124-2087">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ae124-2088">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="ae124-2088">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ae124-2089">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="ae124-2089">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ae124-2090">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="ae124-2090">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-2091">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-2091">CosmosDB</span></span>

* <span data-ttu-id="ae124-2092">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="ae124-2092">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ae124-2093">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2093">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ae124-2094">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ae124-2094">Data Lake Analytics</span></span>

* <span data-ttu-id="ae124-2095">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2095">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ae124-2096">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2096">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ae124-2097">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2097">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ae124-2098">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ae124-2098">Data Lake Store</span></span>

* <span data-ttu-id="ae124-2099">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2099">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ae124-2100">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="ae124-2100">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ae124-2101">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ae124-2101">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ae124-2102">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="ae124-2102">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ae124-2103">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="ae124-2103">Interactive</span></span>

* <span data-ttu-id="ae124-2104">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-2104">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ae124-2105">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-2105">Increased test coverage</span></span>
* <span data-ttu-id="ae124-2106">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-2106">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ae124-2107">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="ae124-2107">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ae124-2108">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="ae124-2108">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ae124-2109">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="ae124-2109">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ae124-2110">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="ae124-2110">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ae124-2111">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2111">Added `--progress` flag</span></span>
* <span data-ttu-id="ae124-2112">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-2112">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ae124-2113">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="ae124-2113">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ae124-2114">IoT</span><span class="sxs-lookup"><span data-stu-id="ae124-2114">IoT</span></span>

* <span data-ttu-id="ae124-2115">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="ae124-2115">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ae124-2116">(3934)</span><span class="sxs-lookup"><span data-stu-id="ae124-2116">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ae124-2117">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="ae124-2117">Key vault</span></span>

* <span data-ttu-id="ae124-2118">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="ae124-2118">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ae124-2119">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ae124-2119">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ae124-2120">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ae124-2120">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ae124-2121">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ae124-2121">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ae124-2122">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ae124-2122">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ae124-2123">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="ae124-2123">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ae124-2124">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="ae124-2124">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ae124-2125">(3307)</span><span class="sxs-lookup"><span data-stu-id="ae124-2125">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ae124-2126">Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-2126">Lab</span></span>

* <span data-ttu-id="ae124-2127">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2127">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ae124-2128">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2128">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-2129">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-2129">Monitor</span></span>

* <span data-ttu-id="ae124-2130">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="ae124-2130">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ae124-2131">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-2131">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ae124-2132">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-2132">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ae124-2133">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-2133">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ae124-2134">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="ae124-2134">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ae124-2135">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="ae124-2135">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ae124-2136">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="ae124-2136">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ae124-2137">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="ae124-2137">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ae124-2138">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae124-2138">`location` no longer required</span></span>
  * <span data-ttu-id="ae124-2139">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="ae124-2139">Add name and ID support for target</span></span>
  * <span data-ttu-id="ae124-2140">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="ae124-2140">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ae124-2141">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="ae124-2141">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ae124-2142">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ae124-2142">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ae124-2143">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="ae124-2143">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ae124-2144">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="ae124-2144">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ae124-2145">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2145">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ae124-2146">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-2146">Network</span></span>

* <span data-ttu-id="ae124-2147">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2147">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ae124-2148">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2148">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ae124-2149">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="ae124-2149">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ae124-2150">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="ae124-2150">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ae124-2151">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="ae124-2151">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ae124-2152">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2152">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ae124-2153">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="ae124-2153">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ae124-2154">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="ae124-2154">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ae124-2155">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="ae124-2155">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ae124-2156">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="ae124-2156">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ae124-2157">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2157">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ae124-2158">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2158">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ae124-2159">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="ae124-2159">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ae124-2160">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2160">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ae124-2161">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2161">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ae124-2162">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-2162">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ae124-2163">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="ae124-2163">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ae124-2164">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-2164">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ae124-2165">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2165">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ae124-2166">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-2166">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ae124-2167">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="ae124-2167">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ae124-2168">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="ae124-2168">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ae124-2169">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-2169">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ae124-2170">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="ae124-2170">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ae124-2171">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="ae124-2171">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ae124-2172">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="ae124-2172">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ae124-2173">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="ae124-2173">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-2174">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-2174">Profile</span></span>

* <span data-ttu-id="ae124-2175">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="ae124-2175">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ae124-2176">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="ae124-2176">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ae124-2177">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="ae124-2177">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ae124-2178">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2178">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ae124-2179">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="ae124-2179">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ae124-2180">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ae124-2180">RDBMS</span></span>

* <span data-ttu-id="ae124-2181">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="ae124-2181">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ae124-2182">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="ae124-2182">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ae124-2183">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="ae124-2183">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ae124-2184">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="ae124-2184">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-2185">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-2185">Resource</span></span>

* <span data-ttu-id="ae124-2186">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-2186">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ae124-2187">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="ae124-2187">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ae124-2188">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-2188">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ae124-2189">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="ae124-2189">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ae124-2190">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="ae124-2190">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ae124-2191">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="ae124-2191">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ae124-2192">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="ae124-2192">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ae124-2193">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2193">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ae124-2194">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-2194">Role</span></span>

* <span data-ttu-id="ae124-2195">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="ae124-2195">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ae124-2196">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="ae124-2196">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ae124-2197">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="ae124-2197">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ae124-2198">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="ae124-2198">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ae124-2199">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2199">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ae124-2200">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ae124-2200">Service Fabric</span></span>
* <span data-ttu-id="ae124-2201">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="ae124-2201">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ae124-2202">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="ae124-2202">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ae124-2203">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="ae124-2203">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-2204">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-2204">SQL</span></span>

* <span data-ttu-id="ae124-2205">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-2205">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ae124-2206">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="ae124-2206">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ae124-2207">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2207">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-2208">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-2208">Storage</span></span>

* <span data-ttu-id="ae124-2209">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="ae124-2209">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ae124-2210">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ae124-2210">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ae124-2211">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="ae124-2211">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ae124-2212">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ae124-2212">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ae124-2213">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="ae124-2213">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ae124-2214">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="ae124-2214">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-2215">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-2215">VM</span></span>

* <span data-ttu-id="ae124-2216">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="ae124-2216">Support configuring nsg</span></span>
* <span data-ttu-id="ae124-2217">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-2217">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ae124-2218">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="ae124-2218">Support managed service identities</span></span>
* <span data-ttu-id="ae124-2219">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="ae124-2219">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ae124-2220">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="ae124-2220">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ae124-2221">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-2221">May 10, 2017</span></span>

<span data-ttu-id="ae124-2222">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ae124-2222">Version 2.0.6</span></span>

* <span data-ttu-id="ae124-2223">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="ae124-2223">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ae124-2224">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="ae124-2224">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ae124-2225">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="ae124-2225">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ae124-2226">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-2226">Include Cognitive Services module</span></span>
* <span data-ttu-id="ae124-2227">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-2227">Include Service Fabric module</span></span>
* <span data-ttu-id="ae124-2228">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="ae124-2228">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ae124-2229">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="ae124-2229">Add support for CDN commands</span></span>
* <span data-ttu-id="ae124-2230">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="ae124-2230">Remove Container module</span></span>
* <span data-ttu-id="ae124-2231">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="ae124-2231">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ae124-2232">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ae124-2232">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ae124-2233">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-2233">Core</span></span>

* <span data-ttu-id="ae124-2234">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="ae124-2234">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ae124-2235">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="ae124-2235">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ae124-2236">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="ae124-2236">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ae124-2237">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="ae124-2237">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ae124-2238">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="ae124-2238">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ae124-2239">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="ae124-2239">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ae124-2240">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="ae124-2240">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ae124-2241">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="ae124-2241">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ae124-2242">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="ae124-2242">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ae124-2243">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="ae124-2243">core: Improved performance</span></span>
* <span data-ttu-id="ae124-2244">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="ae124-2244">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ae124-2245">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="ae124-2245">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-2246">ACS</span></span>

* <span data-ttu-id="ae124-2247">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae124-2247">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ae124-2248">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="ae124-2248">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ae124-2249">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="ae124-2249">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ae124-2250">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="ae124-2250">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-2251">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-2251">AppService</span></span>

* <span data-ttu-id="ae124-2252">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="ae124-2252">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ae124-2253">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="ae124-2253">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ae124-2254">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="ae124-2254">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ae124-2255">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="ae124-2255">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ae124-2256">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="ae124-2256">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ae124-2257">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="ae124-2257">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ae124-2258">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="ae124-2258">support slot swap with preview</span></span>
* <span data-ttu-id="ae124-2259">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="ae124-2259">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ae124-2260">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="ae124-2260">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ae124-2261">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ae124-2261">CosmosDB</span></span>

* <span data-ttu-id="ae124-2262">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="ae124-2262">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ae124-2263">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="ae124-2263">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ae124-2264">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="ae124-2264">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ae124-2265">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="ae124-2265">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ae124-2266">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ae124-2266">Data Lake Analytics</span></span>

* <span data-ttu-id="ae124-2267">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="ae124-2267">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ae124-2268">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="ae124-2268">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ae124-2269">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="ae124-2269">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ae124-2270">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="ae124-2270">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ae124-2271">Table</span><span class="sxs-lookup"><span data-stu-id="ae124-2271">Table</span></span>
  * <span data-ttu-id="ae124-2272">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="ae124-2272">Table valued function</span></span>
  * <span data-ttu-id="ae124-2273">Sicht</span><span class="sxs-lookup"><span data-stu-id="ae124-2273">View</span></span>
  * <span data-ttu-id="ae124-2274">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="ae124-2274">Table Statistics.</span></span> <span data-ttu-id="ae124-2275">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="ae124-2275">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ae124-2276">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ae124-2276">Data Lake Store</span></span>

* <span data-ttu-id="ae124-2277">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-2277">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ae124-2278">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ae124-2278">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ae124-2279">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="ae124-2279">missed help for access show.</span></span> <span data-ttu-id="ae124-2280">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="ae124-2280">adding it.</span></span> <span data-ttu-id="ae124-2281">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ae124-2281">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ae124-2282">Suchen</span><span class="sxs-lookup"><span data-stu-id="ae124-2282">Find</span></span>

* <span data-ttu-id="ae124-2283">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="ae124-2283">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ae124-2284">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ae124-2284">KeyVault</span></span>

* <span data-ttu-id="ae124-2285">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="ae124-2285">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ae124-2286">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="ae124-2286">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ae124-2287">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="ae124-2287">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ae124-2288">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="ae124-2288">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ae124-2289">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="ae124-2289">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ae124-2290">Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-2290">Lab</span></span>

* <span data-ttu-id="ae124-2291">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="ae124-2291">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ae124-2292">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-2292">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ae124-2293">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="ae124-2293">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ae124-2294">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="ae124-2294">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ae124-2295">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="ae124-2295">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ae124-2296">Überwachen</span><span class="sxs-lookup"><span data-stu-id="ae124-2296">Monitor</span></span>

* <span data-ttu-id="ae124-2297">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="ae124-2297">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ae124-2298">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="ae124-2298">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ae124-2299">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-2299">Network</span></span>

* <span data-ttu-id="ae124-2300">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="ae124-2300">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ae124-2301">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="ae124-2301">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ae124-2302">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="ae124-2302">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ae124-2303">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="ae124-2303">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ae124-2304">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="ae124-2304">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ae124-2305">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="ae124-2305">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ae124-2306">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="ae124-2306">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ae124-2307">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="ae124-2307">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ae124-2308">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="ae124-2308">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ae124-2309">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="ae124-2309">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ae124-2310">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="ae124-2310">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ae124-2311">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ae124-2311">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ae124-2312">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="ae124-2312">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ae124-2313">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="ae124-2313">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ae124-2314">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="ae124-2314">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ae124-2315">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="ae124-2315">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ae124-2316">Profil</span><span class="sxs-lookup"><span data-stu-id="ae124-2316">Profile</span></span>

* <span data-ttu-id="ae124-2317">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="ae124-2317">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ae124-2318">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="ae124-2318">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ae124-2319">Redis</span><span class="sxs-lookup"><span data-stu-id="ae124-2319">Redis</span></span>

* <span data-ttu-id="ae124-2320">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="ae124-2320">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ae124-2321">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="ae124-2321">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ae124-2322">Resource</span><span class="sxs-lookup"><span data-stu-id="ae124-2322">Resource</span></span>

* <span data-ttu-id="ae124-2323">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="ae124-2323">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ae124-2324">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="ae124-2324">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ae124-2325">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="ae124-2325">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ae124-2326">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="ae124-2326">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ae124-2327">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ae124-2327">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ae124-2328">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="ae124-2328">Add docs for az lock update.</span></span> <span data-ttu-id="ae124-2329">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ae124-2329">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ae124-2330">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="ae124-2330">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ae124-2331">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ae124-2331">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ae124-2332">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="ae124-2332">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ae124-2333">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ae124-2333">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ae124-2334">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="ae124-2334">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ae124-2335">Rolle</span><span class="sxs-lookup"><span data-stu-id="ae124-2335">Role</span></span>

* <span data-ttu-id="ae124-2336">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="ae124-2336">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ae124-2337">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="ae124-2337">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ae124-2338">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="ae124-2338">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ae124-2339">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="ae124-2339">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ae124-2340">SQL</span><span class="sxs-lookup"><span data-stu-id="ae124-2340">SQL</span></span>

* <span data-ttu-id="ae124-2341">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="ae124-2341">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ae124-2342">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="ae124-2342">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ae124-2343">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-2343">Storage</span></span>

* <span data-ttu-id="ae124-2344">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="ae124-2344">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ae124-2345">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="ae124-2345">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ae124-2346">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="ae124-2346">Add support for large block blob upload</span></span>
* <span data-ttu-id="ae124-2347">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="ae124-2347">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-2348">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-2348">VM</span></span>

* <span data-ttu-id="ae124-2349">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="ae124-2349">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ae124-2350">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="ae124-2350">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ae124-2351">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ae124-2351">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ae124-2352">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ae124-2352">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ae124-2353">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="ae124-2353">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ae124-2354">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="ae124-2354">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ae124-2355">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="ae124-2355">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ae124-2356">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-2356">April 3, 2017</span></span>

<span data-ttu-id="ae124-2357">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ae124-2357">Version 2.0.2</span></span>

<span data-ttu-id="ae124-2358">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="ae124-2358">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="ae124-2359">Core</span><span class="sxs-lookup"><span data-stu-id="ae124-2359">Core</span></span>

* <span data-ttu-id="ae124-2360">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="ae124-2360">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ae124-2361">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="ae124-2361">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ae124-2362">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="ae124-2362">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ae124-2363">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ae124-2363">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ae124-2364">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="ae124-2364">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ae124-2365">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="ae124-2365">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ae124-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="ae124-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ae124-2367">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="ae124-2367">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ae124-2368">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="ae124-2368">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ae124-2369">ACS</span><span class="sxs-lookup"><span data-stu-id="ae124-2369">ACS</span></span>

* <span data-ttu-id="ae124-2370">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="ae124-2370">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ae124-2371">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="ae124-2371">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ae124-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="ae124-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ae124-2373">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="ae124-2373">Add support for windows clusters.</span></span> <span data-ttu-id="ae124-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="ae124-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ae124-2375">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="ae124-2375">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ae124-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="ae124-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ae124-2377">AppService</span><span class="sxs-lookup"><span data-stu-id="ae124-2377">AppService</span></span>

* <span data-ttu-id="ae124-2378">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="ae124-2378">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ae124-2379">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="ae124-2379">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ae124-2380">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="ae124-2380">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ae124-2381">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="ae124-2381">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ae124-2382">DataLake</span><span class="sxs-lookup"><span data-stu-id="ae124-2382">DataLake</span></span>

* <span data-ttu-id="ae124-2383">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-2383">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ae124-2384">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="ae124-2384">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ae124-2385">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ae124-2385">DocuemntDB</span></span>

* <span data-ttu-id="ae124-2386">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="ae124-2386">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ae124-2387">VM</span><span class="sxs-lookup"><span data-stu-id="ae124-2387">VM</span></span>

* <span data-ttu-id="ae124-2388">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="ae124-2388">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ae124-2389">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="ae124-2389">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ae124-2390">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="ae124-2390">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ae124-2391">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ae124-2391">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ae124-2392">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="ae124-2392">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ae124-2393">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="ae124-2393">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="ae124-2394">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="ae124-2394">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ae124-2395">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="ae124-2395">February 27, 2017</span></span>

<span data-ttu-id="ae124-2396">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ae124-2396">Version 2.0.0</span></span>

<span data-ttu-id="ae124-2397">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="ae124-2397">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ae124-2398">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="ae124-2398">Container Service (acs)</span></span>
- <span data-ttu-id="ae124-2399">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="ae124-2399">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ae124-2400">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="ae124-2400">Networking</span></span>
- <span data-ttu-id="ae124-2401">Storage</span><span class="sxs-lookup"><span data-stu-id="ae124-2401">Storage</span></span>

<span data-ttu-id="ae124-2402">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="ae124-2402">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ae124-2403">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="ae124-2403">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ae124-2404">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="ae124-2404">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="ae124-2405">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="ae124-2405">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ae124-2406">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ae124-2406">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ae124-2407">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="ae124-2407">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ae124-2408">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="ae124-2408">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ae124-2409">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="ae124-2409">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ae124-2410">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="ae124-2410">Provide feedback from the command line with the `az feedback` command</span></span>


---
title: Azure CLI 2.0-Versionshinweise
description: Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/28/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 62e57d048666f478b670f182bb9348dba90de6a0
ms.sourcegitcommit: 8f060bc009278eafc0ed448bad4b7d08c742ff63
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/29/2018
ms.locfileid: "43145089"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="01b16-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="01b16-103">Azure CLI 2.0 release notes</span></span>

## <a name="auguest-28-2018"></a><span data-ttu-id="01b16-104">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-104">Auguest 28, 2018</span></span>

<span data-ttu-id="01b16-105">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="01b16-105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="01b16-106">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-106">Core</span></span>

* <span data-ttu-id="01b16-107">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="01b16-107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="01b16-108">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-109">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-109">ACR</span></span>

* <span data-ttu-id="01b16-110">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="01b16-111">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="01b16-111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-112">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-112">ACS</span></span>

* <span data-ttu-id="01b16-113">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="01b16-113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="01b16-114">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="01b16-114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-115">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-115">AppService</span></span>

* <span data-ttu-id="01b16-116">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="01b16-117">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="01b16-118">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="01b16-119">Backup</span><span class="sxs-lookup"><span data-stu-id="01b16-119">Backup</span></span>

* <span data-ttu-id="01b16-120">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="01b16-121">Botdienst</span><span class="sxs-lookup"><span data-stu-id="01b16-121">Bot Service</span></span>

* <span data-ttu-id="01b16-122">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="01b16-122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="01b16-123">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="01b16-123">Cognitive Services</span></span>

* <span data-ttu-id="01b16-124">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="01b16-124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-125">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-125">IoT</span></span>

* <span data-ttu-id="01b16-126">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-127">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-127">Monitor</span></span>

* <span data-ttu-id="01b16-128">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="01b16-129">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="01b16-130">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-130">Network</span></span>

* <span data-ttu-id="01b16-131">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-132">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-132">Resource</span></span>

* <span data-ttu-id="01b16-133">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-134">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-134">Storage</span></span>

* <span data-ttu-id="01b16-135">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-136">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-136">VM</span></span>

* <span data-ttu-id="01b16-137">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="01b16-137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="01b16-138">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="01b16-138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="01b16-139">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-139">Auguest 14, 2018</span></span>

<span data-ttu-id="01b16-140">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="01b16-140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="01b16-141">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-141">Core</span></span>

* <span data-ttu-id="01b16-142">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="01b16-143">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="01b16-144">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="01b16-144">Telemetry</span></span>

* <span data-ttu-id="01b16-145">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="01b16-145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-146">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-146">ACR</span></span>

* <span data-ttu-id="01b16-147">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="01b16-148">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-149">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-149">ACS</span></span>

* <span data-ttu-id="01b16-150">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="01b16-151">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="01b16-151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="01b16-152">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="01b16-152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="01b16-153">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="01b16-153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="01b16-154">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="01b16-154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="01b16-155">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-155">AppService</span></span>

* <span data-ttu-id="01b16-156">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="01b16-156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="01b16-157">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="01b16-158">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-158">BatchAI</span></span>

* <span data-ttu-id="01b16-159">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="01b16-159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="01b16-160">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-160">Container</span></span>

* <span data-ttu-id="01b16-161">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="01b16-162">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-162">IoT</span></span>

* <span data-ttu-id="01b16-163">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="01b16-164">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="01b16-164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="01b16-165">Iot Central</span><span class="sxs-lookup"><span data-stu-id="01b16-165">Iot Central</span></span>

* <span data-ttu-id="01b16-166">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-167">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-167">KeyVault</span></span>


* <span data-ttu-id="01b16-168">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="01b16-169">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="01b16-170">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="01b16-171">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="01b16-172">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="01b16-173">Relay</span><span class="sxs-lookup"><span data-stu-id="01b16-173">Relay</span></span>

* <span data-ttu-id="01b16-174">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-175">Sql</span><span class="sxs-lookup"><span data-stu-id="01b16-175">Sql</span></span>

* <span data-ttu-id="01b16-176">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-177">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-177">Storage</span></span>

* <span data-ttu-id="01b16-178">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="01b16-178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="01b16-179">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="01b16-179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="01b16-180">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="01b16-181">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="01b16-181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="01b16-182">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="01b16-182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-183">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-183">VM</span></span>

* <span data-ttu-id="01b16-184">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="01b16-185">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-185">July 31, 2018</span></span>

<span data-ttu-id="01b16-186">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="01b16-186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-187">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-187">ACR</span></span>

* <span data-ttu-id="01b16-188">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="01b16-189">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-190">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-190">ACS</span></span>

* <span data-ttu-id="01b16-191">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-192">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-192">Batch</span></span>

* <span data-ttu-id="01b16-193">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="01b16-193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="01b16-194">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-194">Container</span></span>

* <span data-ttu-id="01b16-195">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="01b16-196">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-196">Network</span></span>

* <span data-ttu-id="01b16-197">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="01b16-198">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-198">Resource</span></span>

* <span data-ttu-id="01b16-199">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="01b16-199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="01b16-200">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="01b16-200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="01b16-201">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-201">Role</span></span>

* <span data-ttu-id="01b16-202">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="01b16-203">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="01b16-203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="01b16-204">Suchen,</span><span class="sxs-lookup"><span data-stu-id="01b16-204">Search</span></span>

* <span data-ttu-id="01b16-205">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="01b16-206">Service Bus</span><span class="sxs-lookup"><span data-stu-id="01b16-206">Service Bus</span></span>

* <span data-ttu-id="01b16-207">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="01b16-207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="01b16-208">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="01b16-209">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="01b16-209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="01b16-210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="01b16-210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-211">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-211">Storage</span></span>

* <span data-ttu-id="01b16-212">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="01b16-213">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-214">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-214">VM</span></span>

* <span data-ttu-id="01b16-215">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="01b16-216">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="01b16-217">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="01b16-218">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="01b16-218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="01b16-219">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-219">July 18, 2018</span></span>

<span data-ttu-id="01b16-220">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="01b16-220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="01b16-221">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-221">Core</span></span>

* <span data-ttu-id="01b16-222">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="01b16-223">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="01b16-224">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="01b16-224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-225">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-225">ACR</span></span>

* <span data-ttu-id="01b16-226">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="01b16-227">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="01b16-228">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="01b16-228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="01b16-229">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-230">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-230">ACS</span></span>

* <span data-ttu-id="01b16-231">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="01b16-231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-232">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-232">AppService</span></span>

* <span data-ttu-id="01b16-233">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-234">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-234">Batch</span></span>

* <span data-ttu-id="01b16-235">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="01b16-235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="01b16-236">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="01b16-237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-237">Batch AI</span></span>

* <span data-ttu-id="01b16-238">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="01b16-239">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-239">Container</span></span>

* <span data-ttu-id="01b16-240">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="01b16-241">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="01b16-242">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-242">Network</span></span>

* <span data-ttu-id="01b16-243">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="01b16-244">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-244">Added `network nic wait`</span></span>
* <span data-ttu-id="01b16-245">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="01b16-246">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="01b16-246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="01b16-247">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-247">Resource</span></span>

* <span data-ttu-id="01b16-248">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="01b16-249">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="01b16-250">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-250">Added `deployment wait` command</span></span>
* <span data-ttu-id="01b16-251">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-252">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-252">SQL</span></span>

* <span data-ttu-id="01b16-253">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="01b16-254">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="01b16-254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="01b16-255">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-256">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-256">Storage</span></span>

* <span data-ttu-id="01b16-257">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-258">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-258">VM</span></span>

* <span data-ttu-id="01b16-259">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="01b16-260">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="01b16-261">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="01b16-262">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-262">July 3, 2018</span></span>

<span data-ttu-id="01b16-263">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="01b16-263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="01b16-264">AKS</span><span class="sxs-lookup"><span data-stu-id="01b16-264">AKS</span></span>

* <span data-ttu-id="01b16-265">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="01b16-266">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-266">July 3, 2018</span></span>

<span data-ttu-id="01b16-267">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="01b16-267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="01b16-268">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-268">Core</span></span>

* <span data-ttu-id="01b16-269">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-270">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-270">ACR</span></span>

* <span data-ttu-id="01b16-271">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-271">Added polling build status</span></span>
* <span data-ttu-id="01b16-272">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="01b16-273">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-274">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-274">ACS</span></span>

* <span data-ttu-id="01b16-275">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="01b16-275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="01b16-276">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="01b16-276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="01b16-277">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="01b16-277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="01b16-278">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-278">Added `--listen-port` support</span></span>
* <span data-ttu-id="01b16-279">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="01b16-279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="01b16-280">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="01b16-280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="01b16-281">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-282">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-282">AppService</span></span>

* <span data-ttu-id="01b16-283">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="01b16-284">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="01b16-285">Backup</span><span class="sxs-lookup"><span data-stu-id="01b16-285">Backup</span></span>

* <span data-ttu-id="01b16-286">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="01b16-287">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-287">BatchAI</span></span>

* <span data-ttu-id="01b16-288">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="01b16-289">Cloud</span><span class="sxs-lookup"><span data-stu-id="01b16-289">Cloud</span></span>

* <span data-ttu-id="01b16-290">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="01b16-291">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-291">Container</span></span>

* <span data-ttu-id="01b16-292">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="01b16-293">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="01b16-294">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-295">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-295">Extension</span></span>

* <span data-ttu-id="01b16-296">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="01b16-296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="01b16-297">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-297">Network</span></span>

* <span data-ttu-id="01b16-298">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="01b16-298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="01b16-299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="01b16-299">Rdbms</span></span>

* <span data-ttu-id="01b16-300">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-301">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-301">Resource</span></span>

* <span data-ttu-id="01b16-302">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-303">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-303">VM</span></span>

* <span data-ttu-id="01b16-304">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="01b16-305">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-305">June 25, 2018</span></span>

<span data-ttu-id="01b16-306">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="01b16-306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="01b16-307">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="01b16-307">CLI</span></span>

* <span data-ttu-id="01b16-308">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="01b16-308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="01b16-309">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-309">June 19, 2018</span></span>

<span data-ttu-id="01b16-310">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="01b16-310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="01b16-311">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-311">Core</span></span>

* <span data-ttu-id="01b16-312">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-313">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-313">ACR</span></span>

* <span data-ttu-id="01b16-314">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="01b16-315">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="01b16-315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-316">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-316">ACS</span></span>

* <span data-ttu-id="01b16-317">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="01b16-317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="01b16-318">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-318">Added `--update` support</span></span>
* <span data-ttu-id="01b16-319">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="01b16-320">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="01b16-321">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="01b16-322">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="01b16-322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="01b16-323">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="01b16-324">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-325">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-325">AppService</span></span>

* <span data-ttu-id="01b16-326">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="01b16-327">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-328">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-328">Batch</span></span>

* <span data-ttu-id="01b16-329">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="01b16-330">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-330">Batch AI</span></span>

* <span data-ttu-id="01b16-331">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-331">Added support for workspaces.</span></span> <span data-ttu-id="01b16-332">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="01b16-332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="01b16-333">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-333">Added support for experiments.</span></span> <span data-ttu-id="01b16-334">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="01b16-334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="01b16-335">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="01b16-335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="01b16-336">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="01b16-337">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="01b16-337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="01b16-338">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="01b16-339">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="01b16-339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="01b16-340">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="01b16-340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="01b16-341">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="01b16-342">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="01b16-342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="01b16-343">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="01b16-344">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="01b16-344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="01b16-345">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="01b16-346">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="01b16-346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="01b16-347">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="01b16-348">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="01b16-348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="01b16-349">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="01b16-350">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="01b16-351">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="01b16-352">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="01b16-353">Karten</span><span class="sxs-lookup"><span data-stu-id="01b16-353">Maps</span></span>

* <span data-ttu-id="01b16-354">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="01b16-354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="01b16-355">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-355">Network</span></span>

* <span data-ttu-id="01b16-356">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="01b16-356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="01b16-357">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="01b16-357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="01b16-358">#6502</span><span class="sxs-lookup"><span data-stu-id="01b16-358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="01b16-359">Reservations</span><span class="sxs-lookup"><span data-stu-id="01b16-359">Reservations</span></span>

* <span data-ttu-id="01b16-360">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="01b16-361">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="01b16-362">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="01b16-363">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="01b16-364">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="01b16-365">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="01b16-366">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-366">Role</span></span>

* <span data-ttu-id="01b16-367">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-368">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-368">SQL</span></span>

* <span data-ttu-id="01b16-369">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="01b16-369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-370">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-370">Storage</span></span>

* <span data-ttu-id="01b16-371">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-372">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-372">VM</span></span>

* <span data-ttu-id="01b16-373">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="01b16-373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="01b16-374">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="01b16-375">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="01b16-376">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-376">June 13, 2018</span></span>

<span data-ttu-id="01b16-377">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="01b16-377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="01b16-378">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-378">Core</span></span>

* <span data-ttu-id="01b16-379">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="01b16-379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="01b16-380">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-380">June 13, 2018</span></span>

<span data-ttu-id="01b16-381">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="01b16-381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="01b16-382">AKS</span><span class="sxs-lookup"><span data-stu-id="01b16-382">AKS</span></span>

* <span data-ttu-id="01b16-383">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="01b16-384">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="01b16-385">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="01b16-386">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="01b16-387">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-388">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-388">AppService</span></span>

* <span data-ttu-id="01b16-389">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="01b16-390">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-390">June 5, 2018</span></span>

<span data-ttu-id="01b16-391">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="01b16-391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-392">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-392">Interactive</span></span>

* <span data-ttu-id="01b16-393">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="01b16-394">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-394">June 5, 2018</span></span>

<span data-ttu-id="01b16-395">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="01b16-395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="01b16-396">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-396">Core</span></span>

* <span data-ttu-id="01b16-397">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="01b16-398">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="01b16-398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-399">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-399">ACR</span></span>

* <span data-ttu-id="01b16-400">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="01b16-401">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="01b16-402">AKS</span><span class="sxs-lookup"><span data-stu-id="01b16-402">AKS</span></span>

* <span data-ttu-id="01b16-403">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="01b16-403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-404">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-404">Batch</span></span>

* <span data-ttu-id="01b16-405">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="01b16-405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-406">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-406">IOT</span></span>

* <span data-ttu-id="01b16-407">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="01b16-408">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-408">Network</span></span>

* <span data-ttu-id="01b16-409">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="01b16-409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="01b16-410">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="01b16-410">Policy Insights</span></span>

* <span data-ttu-id="01b16-411">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="01b16-412">ARM</span><span class="sxs-lookup"><span data-stu-id="01b16-412">ARM</span></span>

* <span data-ttu-id="01b16-413">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-414">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-414">SQL</span></span>

* <span data-ttu-id="01b16-415">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="01b16-415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="01b16-416">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="01b16-416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="01b16-417">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-417">Storage</span></span>

* <span data-ttu-id="01b16-418">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="01b16-418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-419">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-419">VM</span></span>

* <span data-ttu-id="01b16-420">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="01b16-420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="01b16-421">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="01b16-422">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="01b16-423">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-423">May 22, 2018</span></span>

<span data-ttu-id="01b16-424">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="01b16-424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="01b16-425">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-425">Core</span></span>

* <span data-ttu-id="01b16-426">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-427">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-427">ACS</span></span>

* <span data-ttu-id="01b16-428">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="01b16-429">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-430">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-430">AppService</span></span>

* <span data-ttu-id="01b16-431">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="01b16-431">Improved generic update commands</span></span>
* <span data-ttu-id="01b16-432">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="01b16-433">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-433">Container</span></span>

* <span data-ttu-id="01b16-434">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="01b16-435">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-436">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-436">Extension</span></span>

* <span data-ttu-id="01b16-437">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="01b16-437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-438">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-438">Interactive</span></span>

* <span data-ttu-id="01b16-439">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="01b16-439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="01b16-440">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="01b16-440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-441">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-441">KeyVault</span></span>

* <span data-ttu-id="01b16-442">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="01b16-442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="01b16-443">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-443">Network</span></span>

* <span data-ttu-id="01b16-444">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="01b16-444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="01b16-445">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="01b16-445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-446">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-446">SQL</span></span>

* <span data-ttu-id="01b16-447">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="01b16-447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="01b16-448">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="01b16-449">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="01b16-450">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="01b16-450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="01b16-451">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="01b16-451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="01b16-452">`requestedServiceObjectiveName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="01b16-453">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="01b16-453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="01b16-454">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-454">`edition`.</span></span> <span data-ttu-id="01b16-455">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="01b16-455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="01b16-456">`elasticPoolName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-456">`elasticPoolName`.</span></span> <span data-ttu-id="01b16-457">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="01b16-457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="01b16-458">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="01b16-458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="01b16-459">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-459">`edition`.</span></span> <span data-ttu-id="01b16-460">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="01b16-460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="01b16-461">`dtu`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-461">`dtu`.</span></span> <span data-ttu-id="01b16-462">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="01b16-462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="01b16-463">`databaseDtuMin`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-463">`databaseDtuMin`.</span></span> <span data-ttu-id="01b16-464">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="01b16-464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="01b16-465">`databaseDtuMax`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-465">`databaseDtuMax`.</span></span> <span data-ttu-id="01b16-466">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="01b16-466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="01b16-467">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="01b16-468">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-469">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-469">Storage</span></span>

* <span data-ttu-id="01b16-470">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="01b16-471">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-472">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-472">VM</span></span>

* <span data-ttu-id="01b16-473">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="01b16-474">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="01b16-474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="01b16-475">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="01b16-476">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="01b16-477">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="01b16-478">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-478">May 7, 2018</span></span>

<span data-ttu-id="01b16-479">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="01b16-479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="01b16-480">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-480">Core</span></span>

* <span data-ttu-id="01b16-481">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="01b16-481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="01b16-482">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="01b16-483">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="01b16-483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="01b16-484">#5591</span><span class="sxs-lookup"><span data-stu-id="01b16-484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="01b16-485">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="01b16-486">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="01b16-486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="01b16-487">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="01b16-487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="01b16-488">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="01b16-488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="01b16-489">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-490">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-490">ACR</span></span>

* <span data-ttu-id="01b16-491">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-491">Added ACR Build commands</span></span>
* <span data-ttu-id="01b16-492">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-492">Improved resource not found error messages</span></span>
* <span data-ttu-id="01b16-493">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="01b16-493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="01b16-494">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="01b16-494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="01b16-495">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="01b16-495">Improved repository commands error messages</span></span>
* <span data-ttu-id="01b16-496">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-497">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-497">ACS</span></span>

* <span data-ttu-id="01b16-498">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="01b16-498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="01b16-499">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="01b16-499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="01b16-500">AMS</span><span class="sxs-lookup"><span data-stu-id="01b16-500">AMS</span></span>

* <span data-ttu-id="01b16-501">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="01b16-501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-502">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-502">Appservice</span></span>

* <span data-ttu-id="01b16-503">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="01b16-503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="01b16-504">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="01b16-505">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="01b16-506">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="01b16-507">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-507">Batch AI</span></span>

* <span data-ttu-id="01b16-508">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="01b16-508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="01b16-509">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="01b16-509">Cognitive Services</span></span>

* <span data-ttu-id="01b16-510">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="01b16-510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="01b16-511">Nutzung</span><span class="sxs-lookup"><span data-stu-id="01b16-511">Consumption</span></span>

* <span data-ttu-id="01b16-512">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="01b16-513">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-513">Container</span></span>

* <span data-ttu-id="01b16-514">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="01b16-515">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="01b16-515">Cosmos DB</span></span>

* <span data-ttu-id="01b16-516">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="01b16-516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="01b16-517">DMS</span><span class="sxs-lookup"><span data-stu-id="01b16-517">DMS</span></span>

* <span data-ttu-id="01b16-518">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01b16-518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-519">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-519">Extension</span></span>

* <span data-ttu-id="01b16-520">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-521">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-521">Interactive</span></span>

* <span data-ttu-id="01b16-522">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="01b16-522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="01b16-523">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="01b16-523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="01b16-524">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="01b16-525">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="01b16-526">Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-526">Lab</span></span>

* <span data-ttu-id="01b16-527">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="01b16-528">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-528">Network</span></span>

* <span data-ttu-id="01b16-529">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="01b16-529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="01b16-530">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-530">Profile</span></span>

* <span data-ttu-id="01b16-531">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="01b16-532">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="01b16-532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="01b16-533">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="01b16-534">Redis</span><span class="sxs-lookup"><span data-stu-id="01b16-534">Redis</span></span>

* <span data-ttu-id="01b16-535">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="01b16-535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="01b16-536">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="01b16-537">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="01b16-537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="01b16-538">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="01b16-538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="01b16-539">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="01b16-540">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-540">Role</span></span>

* <span data-ttu-id="01b16-541">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-542">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-542">Storage</span></span>

* <span data-ttu-id="01b16-543">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="01b16-543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="01b16-544">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="01b16-544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="01b16-545">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="01b16-545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="01b16-546">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="01b16-546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="01b16-547">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="01b16-547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-548">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-548">VM</span></span>

* <span data-ttu-id="01b16-549">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="01b16-550">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="01b16-551">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="01b16-551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="01b16-552">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="01b16-553">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="01b16-553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="01b16-554">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-554">Added write accelerator support</span></span>
* <span data-ttu-id="01b16-555">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="01b16-556">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="01b16-556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="01b16-557">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="01b16-557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="01b16-558">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-558">April 10, 2018</span></span>

<span data-ttu-id="01b16-559">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="01b16-559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-560">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-560">ACR</span></span>

* <span data-ttu-id="01b16-561">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="01b16-561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-562">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-562">ACS</span></span>

* <span data-ttu-id="01b16-563">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-564">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-564">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="01b16-566">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="01b16-567">Batch AI</span><span class="sxs-lookup"><span data-stu-id="01b16-567">BatchAI</span></span>

* <span data-ttu-id="01b16-568">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-568">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="01b16-569">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="01b16-569">Job level mounting</span></span>
 - <span data-ttu-id="01b16-570">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="01b16-570">Environment variables with secret values</span></span>
 - <span data-ttu-id="01b16-571">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="01b16-571">Performance counters settings</span></span>
 - <span data-ttu-id="01b16-572">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="01b16-572">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="01b16-573">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="01b16-573">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="01b16-574">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="01b16-574">Usage and limits reporting</span></span>
 - <span data-ttu-id="01b16-575">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="01b16-575">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="01b16-576">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="01b16-576">Support for custom images</span></span>
 - <span data-ttu-id="01b16-577">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="01b16-578">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="01b16-578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="01b16-579">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="01b16-579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="01b16-580">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="01b16-580">National clouds are supported</span></span>
* <span data-ttu-id="01b16-581">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="01b16-582">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="01b16-582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="01b16-583">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="01b16-584">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="01b16-584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="01b16-585">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="01b16-585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="01b16-586">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="01b16-586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="01b16-587">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="01b16-587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="01b16-588">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="01b16-589">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="01b16-589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="01b16-590">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="01b16-591">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="01b16-591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="01b16-592">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="01b16-592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="01b16-593">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="01b16-593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="01b16-594">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="01b16-594">Billing</span></span>

* <span data-ttu-id="01b16-595">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="01b16-596">Nutzung</span><span class="sxs-lookup"><span data-stu-id="01b16-596">Consumption</span></span>

* <span data-ttu-id="01b16-597">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-597">Added `marketplace` commands</span></span>
* <span data-ttu-id="01b16-598">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="01b16-599">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="01b16-600">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="01b16-601">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="01b16-602">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="01b16-603">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-603">Container</span></span>

* <span data-ttu-id="01b16-604">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="01b16-605">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-606">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-606">Extension</span></span>

* <span data-ttu-id="01b16-607">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-608">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-608">Interactive</span></span>

* <span data-ttu-id="01b16-609">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="01b16-609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="01b16-610">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="01b16-611">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="01b16-612">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-612">Network</span></span>

* <span data-ttu-id="01b16-613">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="01b16-613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="01b16-614">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="01b16-615">#4910</span><span class="sxs-lookup"><span data-stu-id="01b16-615">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="01b16-616">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="01b16-617">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="01b16-618">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="01b16-619">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="01b16-620">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-621">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-621">Profile</span></span>

* <span data-ttu-id="01b16-622">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="01b16-623">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="01b16-624">RDBMS</span><span class="sxs-lookup"><span data-stu-id="01b16-624">RDBMS</span></span>

* <span data-ttu-id="01b16-625">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-625">Added `georestore` command</span></span>
* <span data-ttu-id="01b16-626">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-627">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-627">Resource</span></span>

* <span data-ttu-id="01b16-628">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="01b16-629">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-630">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-630">SQL</span></span>

* <span data-ttu-id="01b16-631">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-632">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-632">Storage</span></span>

* <span data-ttu-id="01b16-633">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-634">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-634">VM</span></span>

* <span data-ttu-id="01b16-635">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="01b16-636">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="01b16-638">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="01b16-639">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="01b16-639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="01b16-640">#5718</span><span class="sxs-lookup"><span data-stu-id="01b16-640">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="01b16-641">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="01b16-641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="01b16-642">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-642">March 27, 2018</span></span>

<span data-ttu-id="01b16-643">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="01b16-643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="01b16-644">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-644">Core</span></span>

* <span data-ttu-id="01b16-645">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="01b16-645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-646">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-646">ACS</span></span>

* <span data-ttu-id="01b16-647">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="01b16-647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-648">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-648">Appservice</span></span>

* <span data-ttu-id="01b16-649">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="01b16-650">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="01b16-651">Backup</span><span class="sxs-lookup"><span data-stu-id="01b16-651">Backup</span></span>

* <span data-ttu-id="01b16-652">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="01b16-653">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="01b16-653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="01b16-654">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="01b16-654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="01b16-655">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="01b16-655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="01b16-656">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-656">Container</span></span>

* <span data-ttu-id="01b16-657">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-657">Added `container exec` command.</span></span> <span data-ttu-id="01b16-658">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="01b16-658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="01b16-659">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="01b16-659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-660">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-660">Extension</span></span>

* <span data-ttu-id="01b16-661">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="01b16-661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="01b16-662">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="01b16-662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="01b16-663">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="01b16-663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-664">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-664">Interactive</span></span>

* <span data-ttu-id="01b16-665">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="01b16-666">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="01b16-667">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="01b16-667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="01b16-668">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="01b16-668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="01b16-669">Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-669">Lab</span></span>

* <span data-ttu-id="01b16-670">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-671">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-671">Monitor</span></span>

* <span data-ttu-id="01b16-672">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="01b16-672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="01b16-673">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="01b16-673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="01b16-674">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="01b16-674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="01b16-675">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-675">Network</span></span>

* <span data-ttu-id="01b16-676">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-677">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-677">Profile</span></span>

* <span data-ttu-id="01b16-678">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="01b16-679">RDBMS</span><span class="sxs-lookup"><span data-stu-id="01b16-679">RDBMS</span></span>

* <span data-ttu-id="01b16-680">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-681">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-681">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="01b16-683">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-683">Role</span></span>

* <span data-ttu-id="01b16-684">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="01b16-685">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="01b16-685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="01b16-686">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="01b16-687">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="01b16-688">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-689">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-689">Storage</span></span>

* <span data-ttu-id="01b16-690">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="01b16-691">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="01b16-691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-692">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-692">VM</span></span>

* <span data-ttu-id="01b16-693">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="01b16-694">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="01b16-695">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="01b16-695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="01b16-696">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="01b16-696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="01b16-697">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-697">March 13, 2018</span></span>

<span data-ttu-id="01b16-698">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="01b16-698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-699">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-699">ACR</span></span>

* <span data-ttu-id="01b16-700">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="01b16-701">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="01b16-702">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-703">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-703">ACS</span></span>

* <span data-ttu-id="01b16-704">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="01b16-705">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="01b16-706">Advisor</span><span class="sxs-lookup"><span data-stu-id="01b16-706">Advisor</span></span>

* <span data-ttu-id="01b16-707">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="01b16-708">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="01b16-709">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="01b16-710">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="01b16-711">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-712">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-712">Appservice</span></span>

* <span data-ttu-id="01b16-713">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="01b16-714">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="01b16-715">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="01b16-715">Eventhubs</span></span>

* <span data-ttu-id="01b16-716">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-717">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-717">Extension</span></span>

* <span data-ttu-id="01b16-718">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="01b16-718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-719">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-719">Interactive</span></span>

* <span data-ttu-id="01b16-720">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="01b16-720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="01b16-721">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="01b16-721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="01b16-722">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="01b16-722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="01b16-723">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-724">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-724">Monitor</span></span>

* <span data-ttu-id="01b16-725">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="01b16-726">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="01b16-727">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="01b16-728">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="01b16-729">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-729">Network</span></span>

* <span data-ttu-id="01b16-730">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="01b16-731">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="01b16-731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="01b16-732">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="01b16-733">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-734">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-734">Profile</span></span>

* <span data-ttu-id="01b16-735">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="01b16-736">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="01b16-737">RDBMS</span><span class="sxs-lookup"><span data-stu-id="01b16-737">RDBMS</span></span>

* <span data-ttu-id="01b16-738">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="01b16-739">Service Bus</span><span class="sxs-lookup"><span data-stu-id="01b16-739">Service Bus</span></span>

* <span data-ttu-id="01b16-740">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-741">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-741">Storage</span></span>

* <span data-ttu-id="01b16-742">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="01b16-742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="01b16-743">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="01b16-743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-744">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-744">VM</span></span>

* <span data-ttu-id="01b16-745">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="01b16-745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="01b16-746">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="01b16-746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="01b16-747">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="01b16-748">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="01b16-749">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-749">February 27, 2018</span></span>

<span data-ttu-id="01b16-750">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="01b16-750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="01b16-751">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-751">Core</span></span>

* <span data-ttu-id="01b16-752">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="01b16-753">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="01b16-754">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-755">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-755">ACS</span></span>

* <span data-ttu-id="01b16-756">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="01b16-757">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="01b16-757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="01b16-758">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="01b16-759">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-760">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-760">Appservice</span></span>

* <span data-ttu-id="01b16-761">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="01b16-761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="01b16-762">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="01b16-762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="01b16-763">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="01b16-763">Cognitive Services</span></span>

* <span data-ttu-id="01b16-764">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="01b16-765">Nutzung</span><span class="sxs-lookup"><span data-stu-id="01b16-765">Consumption</span></span>

* <span data-ttu-id="01b16-766">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="01b16-767">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="01b16-768">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-768">Container</span></span>

* <span data-ttu-id="01b16-769">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="01b16-769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="01b16-770">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-770">Network</span></span>

* <span data-ttu-id="01b16-771">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="01b16-771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-772">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-772">Resource</span></span>

* <span data-ttu-id="01b16-773">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="01b16-773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="01b16-774">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-774">Role</span></span>

* <span data-ttu-id="01b16-775">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-776">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-776">SQL</span></span>

* <span data-ttu-id="01b16-777">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="01b16-777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-778">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-778">Storage</span></span>

* <span data-ttu-id="01b16-779">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-780">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-780">VM</span></span>

* <span data-ttu-id="01b16-781">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="01b16-782">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-782">February 13, 2018</span></span>

<span data-ttu-id="01b16-783">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="01b16-783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="01b16-784">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-784">Core</span></span>

* <span data-ttu-id="01b16-785">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-786">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-786">ACS</span></span>

* <span data-ttu-id="01b16-787">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="01b16-788">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="01b16-789">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="01b16-790">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="01b16-791">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="01b16-792">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="01b16-793">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="01b16-793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="01b16-794">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="01b16-794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-795">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-795">Appservice</span></span>

* <span data-ttu-id="01b16-796">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="01b16-796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="01b16-797">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="01b16-798">CDN</span><span class="sxs-lookup"><span data-stu-id="01b16-798">CDN</span></span>

* <span data-ttu-id="01b16-799">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="01b16-800">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-800">Container</span></span>

* <span data-ttu-id="01b16-801">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="01b16-802">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="01b16-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="01b16-803">CosmosDB</span></span>

* <span data-ttu-id="01b16-804">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-805">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-805">Extension</span></span>

* <span data-ttu-id="01b16-806">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="01b16-807">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="01b16-808">Feedback</span><span class="sxs-lookup"><span data-stu-id="01b16-808">Feedback</span></span>

* <span data-ttu-id="01b16-809">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-810">Interactive</span></span>

* <span data-ttu-id="01b16-811">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="01b16-811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="01b16-812">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-813">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-813">IoT</span></span>

* <span data-ttu-id="01b16-814">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="01b16-814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="01b16-815">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="01b16-815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="01b16-816">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="01b16-817">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-818">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-818">Monitor</span></span>

* <span data-ttu-id="01b16-819">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="01b16-820">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-820">Network</span></span>

* <span data-ttu-id="01b16-821">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="01b16-821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="01b16-822">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-822">Profile</span></span>

* <span data-ttu-id="01b16-823">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="01b16-823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-824">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-824">Resource</span></span>

* <span data-ttu-id="01b16-825">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="01b16-826">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-826">Role</span></span>

* <span data-ttu-id="01b16-827">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-828">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-828">SQL</span></span>

* <span data-ttu-id="01b16-829">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="01b16-830">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-830">Added `sql db rename`</span></span>
* <span data-ttu-id="01b16-831">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-832">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-832">Storage</span></span>

* <span data-ttu-id="01b16-833">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-834">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-834">VM</span></span>

* <span data-ttu-id="01b16-835">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="01b16-836">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="01b16-837">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="01b16-837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="01b16-838">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-838">January 31, 2018</span></span>

<span data-ttu-id="01b16-839">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="01b16-839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="01b16-840">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-840">Core</span></span>

* <span data-ttu-id="01b16-841">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="01b16-842">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="01b16-843">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="01b16-843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="01b16-844">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="01b16-844">Use `--verbose` to see</span></span>
* <span data-ttu-id="01b16-845">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-846">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-846">ACS</span></span>

* <span data-ttu-id="01b16-847">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="01b16-847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="01b16-848">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-849">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-849">Appservice</span></span>

* <span data-ttu-id="01b16-850">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="01b16-850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="01b16-851">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="01b16-852">CDN</span><span class="sxs-lookup"><span data-stu-id="01b16-852">CDN</span></span>

* <span data-ttu-id="01b16-853">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="01b16-854">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="01b16-854">CosmosDB</span></span>

* <span data-ttu-id="01b16-855">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-856">Interactive</span></span>

* <span data-ttu-id="01b16-857">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="01b16-858">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-858">Network</span></span>

* <span data-ttu-id="01b16-859">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="01b16-860">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="01b16-860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="01b16-861">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="01b16-862">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="01b16-863">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="01b16-864">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="01b16-864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="01b16-865">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="01b16-866">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="01b16-867">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="01b16-868">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="01b16-868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-869">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-869">Profile</span></span>

* <span data-ttu-id="01b16-870">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-871">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-871">Resource</span></span>

* <span data-ttu-id="01b16-872">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="01b16-872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-873">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-873">Storage</span></span>

* <span data-ttu-id="01b16-874">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="01b16-875">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="01b16-876">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="01b16-876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="01b16-877">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="01b16-878">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="01b16-878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-879">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-879">VM</span></span>

* <span data-ttu-id="01b16-880">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="01b16-881">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="01b16-881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="01b16-882">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="01b16-883">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="01b16-884">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="01b16-884">January 17, 2018</span></span>

<span data-ttu-id="01b16-885">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="01b16-885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-886">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-886">ACR</span></span>

* <span data-ttu-id="01b16-887">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="01b16-888">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="01b16-888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-889">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-889">ACS</span></span>

* <span data-ttu-id="01b16-890">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="01b16-891">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-892">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-892">Appservice</span></span>

* <span data-ttu-id="01b16-893">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="01b16-893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="01b16-894">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="01b16-895">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="01b16-896">Backup</span><span class="sxs-lookup"><span data-stu-id="01b16-896">Backup</span></span>

* <span data-ttu-id="01b16-897">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="01b16-897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="01b16-898">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="01b16-899">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="01b16-899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="01b16-900">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="01b16-900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="01b16-901">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="01b16-901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-902">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-902">Batch</span></span>

* <span data-ttu-id="01b16-903">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="01b16-903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="01b16-904">Cloud</span><span class="sxs-lookup"><span data-stu-id="01b16-904">Cloud</span></span>

* <span data-ttu-id="01b16-905">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="01b16-905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="01b16-906">Nutzung</span><span class="sxs-lookup"><span data-stu-id="01b16-906">Consumption</span></span>

* <span data-ttu-id="01b16-907">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="01b16-907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="01b16-908">Event Grid</span><span class="sxs-lookup"><span data-stu-id="01b16-908">Event Grid</span></span>

* <span data-ttu-id="01b16-909">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="01b16-909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="01b16-910">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="01b16-910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="01b16-911">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="01b16-912">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="01b16-912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="01b16-913">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="01b16-914">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="01b16-915">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="01b16-916">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-917">Interactive</span><span class="sxs-lookup"><span data-stu-id="01b16-917">Interactive</span></span>

* <span data-ttu-id="01b16-918">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="01b16-918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="01b16-919">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-919">Fixed errors on startup</span></span>
* <span data-ttu-id="01b16-920">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="01b16-920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-921">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-921">IoT</span></span>

* <span data-ttu-id="01b16-922">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-922">Added support for device provisioning service</span></span>
* <span data-ttu-id="01b16-923">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="01b16-924">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="01b16-924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-925">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-925">Monitor</span></span>

* <span data-ttu-id="01b16-926">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="01b16-927">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01b16-927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="01b16-928">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="01b16-929">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-929">Network</span></span>

* <span data-ttu-id="01b16-930">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="01b16-930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="01b16-931">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-932">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-932">Profile</span></span>

* <span data-ttu-id="01b16-933">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="01b16-934">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-934">Role</span></span>

* <span data-ttu-id="01b16-935">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="01b16-935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="01b16-936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="01b16-936">Service Fabric</span></span>

* <span data-ttu-id="01b16-937">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="01b16-938">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-939">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-939">VM</span></span>

* <span data-ttu-id="01b16-940">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="01b16-940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="01b16-941">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="01b16-942">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="01b16-942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="01b16-943">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="01b16-944">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="01b16-945">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="01b16-946">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="01b16-947">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="01b16-948">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-948">December 19, 2017</span></span>

<span data-ttu-id="01b16-949">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="01b16-949">Version 2.0.23</span></span>

* <span data-ttu-id="01b16-950">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="01b16-951">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-951">Container</span></span>

* <span data-ttu-id="01b16-952">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="01b16-953">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-953">Network</span></span>

* <span data-ttu-id="01b16-954">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="01b16-955">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-956">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-956">Storage</span></span>

* <span data-ttu-id="01b16-957">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-958">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-958">VM</span></span>

* <span data-ttu-id="01b16-959">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="01b16-960">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-960">December 5, 2017</span></span>

<span data-ttu-id="01b16-961">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="01b16-961">Version 2.0.22</span></span>

* <span data-ttu-id="01b16-962">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-962">Removed `az component` commands.</span></span> <span data-ttu-id="01b16-963">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="01b16-963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="01b16-964">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-964">Core</span></span>
* <span data-ttu-id="01b16-965">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="01b16-965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="01b16-966">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-967">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-967">ACS</span></span>

* <span data-ttu-id="01b16-968">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="01b16-969">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="01b16-969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="01b16-970">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="01b16-970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="01b16-971">Advisor</span><span class="sxs-lookup"><span data-stu-id="01b16-971">Advisor</span></span>

* <span data-ttu-id="01b16-972">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-973">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-973">Appservice</span></span>

* <span data-ttu-id="01b16-974">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="01b16-974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="01b16-975">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="01b16-975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="01b16-976">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="01b16-977">Nutzung</span><span class="sxs-lookup"><span data-stu-id="01b16-977">Consumption</span></span>

* <span data-ttu-id="01b16-978">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="01b16-979">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-979">Container</span></span>

* <span data-ttu-id="01b16-980">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="01b16-980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-981">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-981">Monitor</span></span>

* <span data-ttu-id="01b16-982">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-983">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-983">Resource</span></span>

* <span data-ttu-id="01b16-984">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="01b16-985">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-985">Role</span></span>

* <span data-ttu-id="01b16-986">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="01b16-987">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="01b16-988">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="01b16-988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-989">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-989">SQL</span></span>

* <span data-ttu-id="01b16-990">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="01b16-991">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-992">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-992">VM</span></span>

* <span data-ttu-id="01b16-993">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="01b16-994">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-994">November 14, 2017</span></span>

<span data-ttu-id="01b16-995">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="01b16-995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-996">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-996">ACR</span></span>

* <span data-ttu-id="01b16-997">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="01b16-998">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-998">ACS</span></span>

* <span data-ttu-id="01b16-999">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="01b16-1000">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="01b16-1000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="01b16-1001">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="01b16-1001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="01b16-1002">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="01b16-1003">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1004">Appservice</span></span>

* <span data-ttu-id="01b16-1005">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="01b16-1006">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="01b16-1007">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="01b16-1008">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="01b16-1009">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="01b16-1010">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="01b16-1010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-1011">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-1011">Batch</span></span>

* <span data-ttu-id="01b16-1012">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="01b16-1012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="01b16-1013">BatchAI</span><span class="sxs-lookup"><span data-stu-id="01b16-1013">Batchai</span></span>

* <span data-ttu-id="01b16-1014">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="01b16-1015">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="01b16-1016">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="01b16-1017">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="01b16-1018">Cloud</span><span class="sxs-lookup"><span data-stu-id="01b16-1018">Cloud</span></span>

* <span data-ttu-id="01b16-1019">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="01b16-1019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="01b16-1020">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-1020">Container</span></span>

* <span data-ttu-id="01b16-1021">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1021">Added support to open multiple ports</span></span>
* <span data-ttu-id="01b16-1022">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1022">Added container group restart policy</span></span>
* <span data-ttu-id="01b16-1023">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="01b16-1024">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="01b16-1025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="01b16-1025">Data Lake Analytics</span></span>

* <span data-ttu-id="01b16-1026">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="01b16-1026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="01b16-1027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="01b16-1027">Data Lake Store</span></span>

* <span data-ttu-id="01b16-1028">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="01b16-1028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-1029">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-1029">Extension</span></span>

* <span data-ttu-id="01b16-1030">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-1030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="01b16-1031">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="01b16-1031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-1032">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-1032">IoT</span></span>

* <span data-ttu-id="01b16-1033">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-1034">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-1034">Monitor</span></span>

* <span data-ttu-id="01b16-1035">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1036">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1036">Network</span></span>

* <span data-ttu-id="01b16-1037">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="01b16-1038">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="01b16-1038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="01b16-1039">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="01b16-1039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="01b16-1040">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="01b16-1041">Reservations</span><span class="sxs-lookup"><span data-stu-id="01b16-1041">Reservations</span></span>

* <span data-ttu-id="01b16-1042">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="01b16-1042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1043">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1043">Resource</span></span>

* <span data-ttu-id="01b16-1044">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-1045">SQL</span></span>

* <span data-ttu-id="01b16-1046">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1047">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1047">Storage</span></span>

* <span data-ttu-id="01b16-1048">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="01b16-1049">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="01b16-1049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="01b16-1050">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="01b16-1050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="01b16-1051">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="01b16-1052">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="01b16-1053">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="01b16-1054">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1055">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1055">VM</span></span>

* <span data-ttu-id="01b16-1056">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="01b16-1056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="01b16-1057">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="01b16-1058">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="01b16-1058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="01b16-1059">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="01b16-1060">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="01b16-1061">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1061">October 24, 2017</span></span>

<span data-ttu-id="01b16-1062">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="01b16-1062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="01b16-1063">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1063">Core</span></span>

* <span data-ttu-id="01b16-1064">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="01b16-1064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-1065">ACR</span></span>

* <span data-ttu-id="01b16-1066">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="01b16-1066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="01b16-1067">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="01b16-1067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="01b16-1068">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1069">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1069">ACS</span></span>

* <span data-ttu-id="01b16-1070">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="01b16-1071">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1072">Appservice</span></span>

* <span data-ttu-id="01b16-1073">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="01b16-1073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="01b16-1074">Komponente</span><span class="sxs-lookup"><span data-stu-id="01b16-1074">Component</span></span>

* <span data-ttu-id="01b16-1075">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-1076">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-1076">Monitor</span></span>

* <span data-ttu-id="01b16-1077">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1078">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1078">Resource</span></span>

* <span data-ttu-id="01b16-1079">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="01b16-1080">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="01b16-1080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1081">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1081">VM</span></span>

* <span data-ttu-id="01b16-1082">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="01b16-1083">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1083">October 9, 2017</span></span>

<span data-ttu-id="01b16-1084">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="01b16-1084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="01b16-1085">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1085">Core</span></span>

* <span data-ttu-id="01b16-1086">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1087">Appservice</span></span>

* <span data-ttu-id="01b16-1088">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-1089">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-1089">Batch</span></span>

* <span data-ttu-id="01b16-1090">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="01b16-1090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="01b16-1091">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="01b16-1092">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="01b16-1093">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="01b16-1094">BatchAI</span><span class="sxs-lookup"><span data-stu-id="01b16-1094">Batchai</span></span>

* <span data-ttu-id="01b16-1095">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-1096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-1096">Keyvault</span></span>

* <span data-ttu-id="01b16-1097">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="01b16-1097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="01b16-1098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="01b16-1098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="01b16-1099">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1099">Network</span></span>

* <span data-ttu-id="01b16-1100">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="01b16-1100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="01b16-1101">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1102">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1102">Resource</span></span>

* <span data-ttu-id="01b16-1103">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="01b16-1104">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="01b16-1105">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="01b16-1106">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1107">Sql</span><span class="sxs-lookup"><span data-stu-id="01b16-1107">Sql</span></span>

* <span data-ttu-id="01b16-1108">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="01b16-1109">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="01b16-1110">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1111">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1111">Storage</span></span>

* <span data-ttu-id="01b16-1112">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1113">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1113">Vm</span></span>

* <span data-ttu-id="01b16-1114">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="01b16-1114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="01b16-1115">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="01b16-1116">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="01b16-1117">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="01b16-1118">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="01b16-1119">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1119">September 22, 2017</span></span>

<span data-ttu-id="01b16-1120">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="01b16-1120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1121">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1121">Resource</span></span>

* <span data-ttu-id="01b16-1122">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="01b16-1123">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="01b16-1124">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="01b16-1125">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="01b16-1125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1126">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1126">Network</span></span>

* <span data-ttu-id="01b16-1127">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="01b16-1128">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="01b16-1129">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="01b16-1130">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="01b16-1131">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="01b16-1132">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="01b16-1133">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1134">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1134">Storage</span></span>

* <span data-ttu-id="01b16-1135">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="01b16-1135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="01b16-1136">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="01b16-1136">Eventgrid</span></span>

* <span data-ttu-id="01b16-1137">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1138">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-1138">SQL</span></span>

* <span data-ttu-id="01b16-1139">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="01b16-1139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="01b16-1140">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01b16-1140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="01b16-1141">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-1142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-1142">Keyvault</span></span>

* <span data-ttu-id="01b16-1143">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1144">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1144">VM</span></span>

* <span data-ttu-id="01b16-1145">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="01b16-1146">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="01b16-1146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="01b16-1147">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="01b16-1148">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="01b16-1149">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="01b16-1150">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1151">ACS</span></span>

* <span data-ttu-id="01b16-1152">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1153">Appservice</span></span>

* <span data-ttu-id="01b16-1154">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="01b16-1154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="01b16-1155">Backup</span><span class="sxs-lookup"><span data-stu-id="01b16-1155">Backup</span></span>

* <span data-ttu-id="01b16-1156">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="01b16-1156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="01b16-1157">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1157">September 11, 2017</span></span>

<span data-ttu-id="01b16-1158">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="01b16-1158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="01b16-1159">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1159">Core</span></span>

* <span data-ttu-id="01b16-1160">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="01b16-1160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="01b16-1161">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="01b16-1161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1162">Acs</span></span>

* <span data-ttu-id="01b16-1163">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="01b16-1164">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1165">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1165">Appservice</span></span>

* <span data-ttu-id="01b16-1166">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="01b16-1166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="01b16-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="01b16-1167">CDN</span></span>

* <span data-ttu-id="01b16-1168">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="01b16-1168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="01b16-1169">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="01b16-1169">Extension</span></span>

* <span data-ttu-id="01b16-1170">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-1170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-1171">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-1171">Keyvault</span></span>

* <span data-ttu-id="01b16-1172">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="01b16-1172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1173">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1173">Network</span></span>

* <span data-ttu-id="01b16-1174">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="01b16-1175">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="01b16-1176">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="01b16-1177">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="01b16-1178">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1179">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1179">Resource</span></span>

* <span data-ttu-id="01b16-1180">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="01b16-1180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="01b16-1181">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="01b16-1181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="01b16-1182">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="01b16-1182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="01b16-1183">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="01b16-1183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-1184">SQL</span></span>

* <span data-ttu-id="01b16-1185">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1186">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1186">VM</span></span>

* <span data-ttu-id="01b16-1187">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="01b16-1188">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="01b16-1188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="01b16-1189">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="01b16-1190">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="01b16-1190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="01b16-1191">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="01b16-1191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="01b16-1192">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1192">August 31, 2017</span></span>

<span data-ttu-id="01b16-1193">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="01b16-1193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-1194">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-1194">Keyvault</span></span>

* <span data-ttu-id="01b16-1195">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="01b16-1195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="01b16-1196">Sf</span><span class="sxs-lookup"><span data-stu-id="01b16-1196">Sf</span></span>

* <span data-ttu-id="01b16-1197">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1198">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1198">Storage</span></span>

* <span data-ttu-id="01b16-1199">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="01b16-1199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="01b16-1200">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="01b16-1200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="01b16-1201">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1201">August 28, 2017</span></span>

<span data-ttu-id="01b16-1202">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="01b16-1202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="01b16-1203">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="01b16-1203">CLI</span></span>

* <span data-ttu-id="01b16-1204">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1205">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1205">ACS</span></span>

* <span data-ttu-id="01b16-1206">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1206">Corrected preview regions</span></span>
* <span data-ttu-id="01b16-1207">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="01b16-1208">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1209">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1209">Appservice</span></span>

* <span data-ttu-id="01b16-1210">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="01b16-1211">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="01b16-1212">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="01b16-1213">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="01b16-1213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="01b16-1214">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-1215">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-1215">IoT</span></span>

* <span data-ttu-id="01b16-1216">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="01b16-1216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1217">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1217">Network</span></span>

* <span data-ttu-id="01b16-1218">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="01b16-1219">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="01b16-1220">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="01b16-1221">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="01b16-1222">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-1223">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-1223">Profile</span></span>

* <span data-ttu-id="01b16-1224">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="01b16-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="01b16-1225">Service Fabric</span></span>

* <span data-ttu-id="01b16-1226">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="01b16-1226">Preview release</span></span>
* <span data-ttu-id="01b16-1227">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="01b16-1228">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="01b16-1229">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1230">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1230">Storage</span></span>

* <span data-ttu-id="01b16-1231">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1231">Enabled setting blob tier</span></span>
* <span data-ttu-id="01b16-1232">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="01b16-1233">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="01b16-1234">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="01b16-1235">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="01b16-1236">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="01b16-1236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1237">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1237">VM</span></span>

* <span data-ttu-id="01b16-1238">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="01b16-1239">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="01b16-1239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="01b16-1240">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="01b16-1241">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="01b16-1241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="01b16-1242">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="01b16-1243">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="01b16-1243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="01b16-1244">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1244">August 15, 2017</span></span>

<span data-ttu-id="01b16-1245">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="01b16-1245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1246">ACS</span></span>

* <span data-ttu-id="01b16-1247">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1248">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1248">Appservice</span></span>

* <span data-ttu-id="01b16-1249">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="01b16-1250">Event Grid</span><span class="sxs-lookup"><span data-stu-id="01b16-1250">Event Grid</span></span>

* <span data-ttu-id="01b16-1251">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="01b16-1252">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1252">August 11, 2017</span></span>

<span data-ttu-id="01b16-1253">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="01b16-1253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1254">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1254">ACS</span></span>

* <span data-ttu-id="01b16-1255">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-1256">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-1256">Batch</span></span>

* <span data-ttu-id="01b16-1257">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="01b16-1258">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="01b16-1259">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="01b16-1260">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="01b16-1260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="01b16-1261">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="01b16-1261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="01b16-1262">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="01b16-1263">Komponente</span><span class="sxs-lookup"><span data-stu-id="01b16-1263">Component</span></span>

* <span data-ttu-id="01b16-1264">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="01b16-1265">Container</span><span class="sxs-lookup"><span data-stu-id="01b16-1265">Container</span></span>

* <span data-ttu-id="01b16-1266">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="01b16-1266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="01b16-1267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="01b16-1267">Data Lake Store</span></span>

* <span data-ttu-id="01b16-1268">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="01b16-1269">Event Grid</span><span class="sxs-lookup"><span data-stu-id="01b16-1269">Event Grid</span></span>

* <span data-ttu-id="01b16-1270">Erste Version</span><span class="sxs-lookup"><span data-stu-id="01b16-1270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1271">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1271">Network</span></span>

* <span data-ttu-id="01b16-1272">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="01b16-1273">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-1273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="01b16-1274">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="01b16-1274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="01b16-1275">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="01b16-1275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-1276">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-1276">Profile</span></span>

* <span data-ttu-id="01b16-1277">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="01b16-1277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1278">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1278">Storage</span></span>

* <span data-ttu-id="01b16-1279">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1280">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1280">VM</span></span>

* <span data-ttu-id="01b16-1281">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="01b16-1282">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="01b16-1283">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="01b16-1284">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="01b16-1284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="01b16-1285">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="01b16-1286">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1286">July 28, 2017</span></span>

<span data-ttu-id="01b16-1287">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="01b16-1287">Version 2.0.12</span></span>

* <span data-ttu-id="01b16-1288">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1288">Added container commands</span></span>
* <span data-ttu-id="01b16-1289">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="01b16-1290">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1290">Core</span></span>

* <span data-ttu-id="01b16-1291">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="01b16-1291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="01b16-1292">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="01b16-1293">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="01b16-1293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="01b16-1294">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="01b16-1294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="01b16-1295">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="01b16-1295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="01b16-1296">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="01b16-1296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="01b16-1297">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="01b16-1297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="01b16-1298">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="01b16-1298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="01b16-1299">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="01b16-1299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="01b16-1300">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-1300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="01b16-1301">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="01b16-1301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="01b16-1302">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="01b16-1302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="01b16-1303">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="01b16-1303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="01b16-1304">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="01b16-1304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="01b16-1305">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="01b16-1305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="01b16-1306">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="01b16-1306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="01b16-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-1307">ACR</span></span>

* <span data-ttu-id="01b16-1308">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="01b16-1309">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="01b16-1310">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="01b16-1311">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="01b16-1312">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="01b16-1313">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1314">ACS</span></span>

* <span data-ttu-id="01b16-1315">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="01b16-1315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1316">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1316">Appservice</span></span>

* <span data-ttu-id="01b16-1317">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="01b16-1317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="01b16-1318">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="01b16-1318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="01b16-1319">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="01b16-1319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="01b16-1320">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="01b16-1320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="01b16-1321">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="01b16-1321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="01b16-1322">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="01b16-1322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="01b16-1323">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="01b16-1323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="01b16-1324">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="01b16-1324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="01b16-1325">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="01b16-1326">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="01b16-1326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="01b16-1327">Batch</span><span class="sxs-lookup"><span data-stu-id="01b16-1327">Batch</span></span>

* <span data-ttu-id="01b16-1328">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="01b16-1329">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="01b16-1330">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="01b16-1331">CDN</span><span class="sxs-lookup"><span data-stu-id="01b16-1331">CDN</span></span>

* <span data-ttu-id="01b16-1332">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="01b16-1332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="01b16-1333">Cloud</span><span class="sxs-lookup"><span data-stu-id="01b16-1333">Cloud</span></span>

* <span data-ttu-id="01b16-1334">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="01b16-1334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="01b16-1335">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="01b16-1335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="01b16-1336">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="01b16-1336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="01b16-1337">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="01b16-1337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="01b16-1338">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="01b16-1338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="01b16-1339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="01b16-1339">CosmosDB</span></span>

* <span data-ttu-id="01b16-1340">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="01b16-1340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="01b16-1341">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="01b16-1342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="01b16-1342">Data Lake Analytics</span></span>

* <span data-ttu-id="01b16-1343">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="01b16-1344">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="01b16-1345">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="01b16-1346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="01b16-1346">Data Lake Store</span></span>

* <span data-ttu-id="01b16-1347">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="01b16-1348">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="01b16-1348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="01b16-1349">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="01b16-1350">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="01b16-1350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="01b16-1351">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="01b16-1351">Interactive</span></span>

* <span data-ttu-id="01b16-1352">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="01b16-1353">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1353">Increased test coverage</span></span>
* <span data-ttu-id="01b16-1354">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="01b16-1355">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="01b16-1355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="01b16-1356">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="01b16-1356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="01b16-1357">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="01b16-1357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="01b16-1358">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="01b16-1358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="01b16-1359">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1359">Added `--progress` flag</span></span>
* <span data-ttu-id="01b16-1360">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="01b16-1361">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="01b16-1361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="01b16-1362">IoT</span><span class="sxs-lookup"><span data-stu-id="01b16-1362">IoT</span></span>

* <span data-ttu-id="01b16-1363">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="01b16-1363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="01b16-1364">(3934)</span><span class="sxs-lookup"><span data-stu-id="01b16-1364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="01b16-1365">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="01b16-1365">Key vault</span></span>

* <span data-ttu-id="01b16-1366">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="01b16-1366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="01b16-1367">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="01b16-1367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="01b16-1368">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="01b16-1368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="01b16-1369">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="01b16-1369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="01b16-1370">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="01b16-1370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="01b16-1371">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="01b16-1371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="01b16-1372">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="01b16-1373">(3307)</span><span class="sxs-lookup"><span data-stu-id="01b16-1373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="01b16-1374">Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-1374">Lab</span></span>

* <span data-ttu-id="01b16-1375">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="01b16-1376">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-1377">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-1377">Monitor</span></span>

* <span data-ttu-id="01b16-1378">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="01b16-1378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="01b16-1379">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="01b16-1380">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="01b16-1381">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="01b16-1382">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="01b16-1382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="01b16-1383">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="01b16-1383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="01b16-1384">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="01b16-1384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="01b16-1385">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="01b16-1385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="01b16-1386">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="01b16-1386">`location` no longer required</span></span>
  * <span data-ttu-id="01b16-1387">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="01b16-1387">Add name and ID support for target</span></span>
  * <span data-ttu-id="01b16-1388">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="01b16-1388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="01b16-1389">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="01b16-1389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="01b16-1390">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="01b16-1391">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="01b16-1391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="01b16-1392">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="01b16-1392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="01b16-1393">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1394">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1394">Network</span></span>

* <span data-ttu-id="01b16-1395">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="01b16-1396">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="01b16-1397">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="01b16-1397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="01b16-1398">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="01b16-1398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="01b16-1399">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="01b16-1399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="01b16-1400">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="01b16-1401">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="01b16-1401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="01b16-1402">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="01b16-1402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="01b16-1403">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="01b16-1403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="01b16-1404">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="01b16-1404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="01b16-1405">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="01b16-1406">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="01b16-1407">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="01b16-1407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="01b16-1408">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="01b16-1409">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="01b16-1410">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="01b16-1411">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="01b16-1412">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-1412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="01b16-1413">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="01b16-1414">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="01b16-1415">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="01b16-1415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="01b16-1416">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="01b16-1416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="01b16-1417">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="01b16-1418">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="01b16-1418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="01b16-1419">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="01b16-1419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="01b16-1420">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="01b16-1420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="01b16-1421">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="01b16-1421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-1422">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-1422">Profile</span></span>

* <span data-ttu-id="01b16-1423">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="01b16-1423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="01b16-1424">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="01b16-1424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="01b16-1425">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="01b16-1425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="01b16-1426">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="01b16-1427">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="01b16-1427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="01b16-1428">RDBMS</span><span class="sxs-lookup"><span data-stu-id="01b16-1428">RDBMS</span></span>

* <span data-ttu-id="01b16-1429">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="01b16-1429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="01b16-1430">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="01b16-1430">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="01b16-1431">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="01b16-1431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="01b16-1432">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="01b16-1432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1433">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1433">Resource</span></span>

* <span data-ttu-id="01b16-1434">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="01b16-1435">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="01b16-1435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="01b16-1436">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="01b16-1437">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="01b16-1437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="01b16-1438">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="01b16-1438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="01b16-1439">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="01b16-1439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="01b16-1440">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="01b16-1440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="01b16-1441">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="01b16-1442">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-1442">Role</span></span>

* <span data-ttu-id="01b16-1443">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="01b16-1443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="01b16-1444">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="01b16-1444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="01b16-1445">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="01b16-1445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="01b16-1446">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="01b16-1446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="01b16-1447">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="01b16-1448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="01b16-1448">Service Fabric</span></span>
* <span data-ttu-id="01b16-1449">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="01b16-1449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="01b16-1450">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="01b16-1450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="01b16-1451">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="01b16-1451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1452">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-1452">SQL</span></span>

* <span data-ttu-id="01b16-1453">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="01b16-1454">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="01b16-1454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="01b16-1455">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1456">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1456">Storage</span></span>

* <span data-ttu-id="01b16-1457">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="01b16-1457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="01b16-1458">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="01b16-1459">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="01b16-1459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="01b16-1460">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="01b16-1460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="01b16-1461">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="01b16-1461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="01b16-1462">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="01b16-1462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1463">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1463">VM</span></span>

* <span data-ttu-id="01b16-1464">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="01b16-1464">Support configuring nsg</span></span>
* <span data-ttu-id="01b16-1465">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-1465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="01b16-1466">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="01b16-1466">Support managed service identities</span></span>
* <span data-ttu-id="01b16-1467">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="01b16-1467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="01b16-1468">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="01b16-1468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="01b16-1469">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1469">May 10, 2017</span></span>

<span data-ttu-id="01b16-1470">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="01b16-1470">Version 2.0.6</span></span>

* <span data-ttu-id="01b16-1471">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="01b16-1471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="01b16-1472">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="01b16-1472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="01b16-1473">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="01b16-1473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="01b16-1474">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1474">Include Cognitive Services module</span></span>
* <span data-ttu-id="01b16-1475">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1475">Include Service Fabric module</span></span>
* <span data-ttu-id="01b16-1476">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="01b16-1476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="01b16-1477">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="01b16-1477">Add support for CDN commands</span></span>
* <span data-ttu-id="01b16-1478">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1478">Remove Container module</span></span>
* <span data-ttu-id="01b16-1479">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="01b16-1479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="01b16-1480">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="01b16-1480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="01b16-1481">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1481">Core</span></span>

* <span data-ttu-id="01b16-1482">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="01b16-1482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="01b16-1483">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="01b16-1483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="01b16-1484">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="01b16-1484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="01b16-1485">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="01b16-1485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="01b16-1486">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="01b16-1486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="01b16-1487">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="01b16-1487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="01b16-1488">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="01b16-1488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="01b16-1489">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="01b16-1489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="01b16-1490">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="01b16-1490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="01b16-1491">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="01b16-1491">core: Improved performance</span></span>
* <span data-ttu-id="01b16-1492">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="01b16-1492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="01b16-1493">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="01b16-1493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1494">ACS</span></span>

* <span data-ttu-id="01b16-1495">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01b16-1495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="01b16-1496">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="01b16-1496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="01b16-1497">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="01b16-1498">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="01b16-1498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1499">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1499">AppService</span></span>

* <span data-ttu-id="01b16-1500">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="01b16-1500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="01b16-1501">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="01b16-1501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="01b16-1502">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="01b16-1502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="01b16-1503">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="01b16-1503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="01b16-1504">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="01b16-1504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="01b16-1505">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="01b16-1505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="01b16-1506">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="01b16-1506">support slot swap with preview</span></span>
* <span data-ttu-id="01b16-1507">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="01b16-1507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="01b16-1508">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="01b16-1508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="01b16-1509">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="01b16-1509">CosmosDB</span></span>

* <span data-ttu-id="01b16-1510">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="01b16-1510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="01b16-1511">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="01b16-1511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="01b16-1512">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="01b16-1512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="01b16-1513">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="01b16-1513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="01b16-1514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="01b16-1514">Data Lake Analytics</span></span>

* <span data-ttu-id="01b16-1515">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="01b16-1515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="01b16-1516">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="01b16-1516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="01b16-1517">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="01b16-1517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="01b16-1518">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="01b16-1518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="01b16-1519">Table</span><span class="sxs-lookup"><span data-stu-id="01b16-1519">Table</span></span>
  * <span data-ttu-id="01b16-1520">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="01b16-1520">Table valued function</span></span>
  * <span data-ttu-id="01b16-1521">Sicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1521">View</span></span>
  * <span data-ttu-id="01b16-1522">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="01b16-1522">Table Statistics.</span></span> <span data-ttu-id="01b16-1523">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="01b16-1523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="01b16-1524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="01b16-1524">Data Lake Store</span></span>

* <span data-ttu-id="01b16-1525">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="01b16-1526">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="01b16-1526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="01b16-1527">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="01b16-1527">missed help for access show.</span></span> <span data-ttu-id="01b16-1528">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="01b16-1528">adding it.</span></span> <span data-ttu-id="01b16-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="01b16-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="01b16-1530">Suchen</span><span class="sxs-lookup"><span data-stu-id="01b16-1530">Find</span></span>

* <span data-ttu-id="01b16-1531">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="01b16-1531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="01b16-1532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b16-1532">KeyVault</span></span>

* <span data-ttu-id="01b16-1533">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="01b16-1533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="01b16-1534">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="01b16-1534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="01b16-1535">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="01b16-1535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="01b16-1536">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="01b16-1536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="01b16-1537">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="01b16-1537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="01b16-1538">Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-1538">Lab</span></span>

* <span data-ttu-id="01b16-1539">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="01b16-1539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="01b16-1540">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-1540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="01b16-1541">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="01b16-1541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="01b16-1542">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="01b16-1542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="01b16-1543">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="01b16-1543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="01b16-1544">Überwachen</span><span class="sxs-lookup"><span data-stu-id="01b16-1544">Monitor</span></span>

* <span data-ttu-id="01b16-1545">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="01b16-1545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="01b16-1546">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="01b16-1546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="01b16-1547">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1547">Network</span></span>

* <span data-ttu-id="01b16-1548">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="01b16-1548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="01b16-1549">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="01b16-1549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="01b16-1550">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="01b16-1550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="01b16-1551">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="01b16-1551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="01b16-1552">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="01b16-1552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="01b16-1553">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="01b16-1553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="01b16-1554">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="01b16-1555">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="01b16-1555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="01b16-1556">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="01b16-1556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="01b16-1557">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="01b16-1557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="01b16-1558">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="01b16-1558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="01b16-1559">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="01b16-1559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="01b16-1560">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="01b16-1560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="01b16-1561">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="01b16-1561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="01b16-1562">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="01b16-1562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="01b16-1563">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="01b16-1563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="01b16-1564">Profil</span><span class="sxs-lookup"><span data-stu-id="01b16-1564">Profile</span></span>

* <span data-ttu-id="01b16-1565">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="01b16-1565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="01b16-1566">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="01b16-1566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="01b16-1567">Redis</span><span class="sxs-lookup"><span data-stu-id="01b16-1567">Redis</span></span>

* <span data-ttu-id="01b16-1568">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="01b16-1569">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="01b16-1569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="01b16-1570">Ressource</span><span class="sxs-lookup"><span data-stu-id="01b16-1570">Resource</span></span>

* <span data-ttu-id="01b16-1571">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="01b16-1571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="01b16-1572">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="01b16-1572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="01b16-1573">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="01b16-1573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="01b16-1574">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="01b16-1574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="01b16-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="01b16-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="01b16-1576">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="01b16-1576">Add docs for az lock update.</span></span> <span data-ttu-id="01b16-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="01b16-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="01b16-1578">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="01b16-1578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="01b16-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="01b16-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="01b16-1580">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="01b16-1580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="01b16-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="01b16-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="01b16-1582">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="01b16-1582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="01b16-1583">Rolle</span><span class="sxs-lookup"><span data-stu-id="01b16-1583">Role</span></span>

* <span data-ttu-id="01b16-1584">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="01b16-1584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="01b16-1585">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="01b16-1585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="01b16-1586">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="01b16-1586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="01b16-1587">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="01b16-1587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="01b16-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="01b16-1588">SQL</span></span>

* <span data-ttu-id="01b16-1589">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="01b16-1589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="01b16-1590">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="01b16-1590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="01b16-1591">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1591">Storage</span></span>

* <span data-ttu-id="01b16-1592">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="01b16-1592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="01b16-1593">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="01b16-1593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="01b16-1594">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="01b16-1594">Add support for large block blob upload</span></span>
* <span data-ttu-id="01b16-1595">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="01b16-1595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1596">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1596">VM</span></span>

* <span data-ttu-id="01b16-1597">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="01b16-1597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="01b16-1598">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="01b16-1598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="01b16-1599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="01b16-1599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="01b16-1600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="01b16-1600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="01b16-1601">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="01b16-1601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="01b16-1602">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="01b16-1602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="01b16-1603">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="01b16-1603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="01b16-1604">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1604">April 3, 2017</span></span>

<span data-ttu-id="01b16-1605">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="01b16-1605">Version 2.0.2</span></span>

<span data-ttu-id="01b16-1606">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="01b16-1607">Core</span><span class="sxs-lookup"><span data-stu-id="01b16-1607">Core</span></span>

* <span data-ttu-id="01b16-1608">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="01b16-1608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="01b16-1609">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="01b16-1609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="01b16-1610">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="01b16-1610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="01b16-1611">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="01b16-1611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="01b16-1612">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="01b16-1612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="01b16-1613">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="01b16-1613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="01b16-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="01b16-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="01b16-1615">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="01b16-1616">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="01b16-1616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="01b16-1617">ACS</span><span class="sxs-lookup"><span data-stu-id="01b16-1617">ACS</span></span>

* <span data-ttu-id="01b16-1618">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="01b16-1618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="01b16-1619">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="01b16-1619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="01b16-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="01b16-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="01b16-1621">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="01b16-1621">Add support for windows clusters.</span></span> <span data-ttu-id="01b16-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="01b16-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="01b16-1623">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="01b16-1623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="01b16-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="01b16-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="01b16-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="01b16-1625">AppService</span></span>

* <span data-ttu-id="01b16-1626">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="01b16-1626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="01b16-1627">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="01b16-1627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="01b16-1628">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="01b16-1628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="01b16-1629">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="01b16-1629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="01b16-1630">DataLake</span><span class="sxs-lookup"><span data-stu-id="01b16-1630">DataLake</span></span>

* <span data-ttu-id="01b16-1631">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="01b16-1632">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="01b16-1632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="01b16-1633">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="01b16-1633">DocuemntDB</span></span>

* <span data-ttu-id="01b16-1634">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="01b16-1634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="01b16-1635">VM</span><span class="sxs-lookup"><span data-stu-id="01b16-1635">VM</span></span>

* <span data-ttu-id="01b16-1636">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="01b16-1636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="01b16-1637">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="01b16-1637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="01b16-1638">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="01b16-1638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="01b16-1639">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="01b16-1639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="01b16-1640">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="01b16-1640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="01b16-1641">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="01b16-1641">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="01b16-1642">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="01b16-1642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="01b16-1643">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="01b16-1643">February 27, 2017</span></span>

<span data-ttu-id="01b16-1644">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="01b16-1644">Version 2.0.0</span></span>

<span data-ttu-id="01b16-1645">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="01b16-1645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="01b16-1646">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="01b16-1646">Container Service (acs)</span></span>
- <span data-ttu-id="01b16-1647">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="01b16-1647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="01b16-1648">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="01b16-1648">Networking</span></span>
- <span data-ttu-id="01b16-1649">Speicher</span><span class="sxs-lookup"><span data-stu-id="01b16-1649">Storage</span></span>

<span data-ttu-id="01b16-1650">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="01b16-1650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="01b16-1651">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="01b16-1651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="01b16-1652">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="01b16-1652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="01b16-1653">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="01b16-1653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="01b16-1654">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="01b16-1654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="01b16-1655">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="01b16-1655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="01b16-1656">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="01b16-1656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="01b16-1657">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="01b16-1657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="01b16-1658">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="01b16-1658">Provide feedback from the command line with the `az feedback` command</span></span>


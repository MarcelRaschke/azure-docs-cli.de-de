---
title: Azure CLI 2.0-Versionshinweise
description: Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8d4f0879a18d2cf99ea7a284155bec86413406f8
ms.sourcegitcommit: da34d0eecf19c676826bd32ab254a92bd0976124
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/19/2018
ms.locfileid: "39138235"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="d11ae-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="d11ae-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="d11ae-104">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-104">July 18, 2018</span></span>

<span data-ttu-id="d11ae-105">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="d11ae-105">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-106">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-106">Core</span></span>

* <span data-ttu-id="d11ae-107">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-107">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="d11ae-108">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-108">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="d11ae-109">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="d11ae-109">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-110">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-110">ACR</span></span>

* <span data-ttu-id="d11ae-111">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-111">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="d11ae-112">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-112">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="d11ae-113">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="d11ae-113">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="d11ae-114">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-114">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-115">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-115">ACS</span></span>

* <span data-ttu-id="d11ae-116">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-116">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-117">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-117">AppService</span></span>

* <span data-ttu-id="d11ae-118">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-118">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-119">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-119">Batch</span></span>

* <span data-ttu-id="d11ae-120">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="d11ae-120">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="d11ae-121">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-121">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d11ae-122">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d11ae-122">Batch AI</span></span>

* <span data-ttu-id="d11ae-123">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-123">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-124">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-124">Container</span></span>

* <span data-ttu-id="d11ae-125">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-125">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="d11ae-126">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-126">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-127">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-127">Network</span></span>

* <span data-ttu-id="d11ae-128">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-128">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="d11ae-129">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-129">Added `network nic wait`</span></span>
* <span data-ttu-id="d11ae-130">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-130">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="d11ae-131">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="d11ae-131">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="d11ae-132">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-132">Resource</span></span>

* <span data-ttu-id="d11ae-133">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-133">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="d11ae-134">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-134">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="d11ae-135">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-135">Added `deployment wait` command</span></span>
* <span data-ttu-id="d11ae-136">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-136">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-137">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-137">SQL</span></span>

* <span data-ttu-id="d11ae-138">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-138">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="d11ae-139">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="d11ae-139">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="d11ae-140">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-140">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-141">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-141">Storage</span></span>

* <span data-ttu-id="d11ae-142">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-142">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-143">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-143">VM</span></span>

* <span data-ttu-id="d11ae-144">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-144">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="d11ae-145">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-145">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="d11ae-146">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-146">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d11ae-147">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-147">July 3, 2018</span></span>

<span data-ttu-id="d11ae-148">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="d11ae-148">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="d11ae-149">AKS</span><span class="sxs-lookup"><span data-stu-id="d11ae-149">AKS</span></span>

* <span data-ttu-id="d11ae-150">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-150">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d11ae-151">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-151">July 3, 2018</span></span>

<span data-ttu-id="d11ae-152">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="d11ae-152">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-153">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-153">Core</span></span>

* <span data-ttu-id="d11ae-154">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-154">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-155">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-155">ACR</span></span>

* <span data-ttu-id="d11ae-156">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-156">Added polling build status</span></span>
* <span data-ttu-id="d11ae-157">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-157">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="d11ae-158">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-158">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-159">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-159">ACS</span></span>

* <span data-ttu-id="d11ae-160">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d11ae-160">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="d11ae-161">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-161">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="d11ae-162">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-162">Updated options for `aks browse` command.</span></span> <span data-ttu-id="d11ae-163">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-163">Added `--listen-port` support</span></span>
* <span data-ttu-id="d11ae-164">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-164">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="d11ae-165">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="d11ae-165">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="d11ae-166">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-166">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-167">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-167">AppService</span></span>

* <span data-ttu-id="d11ae-168">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-168">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="d11ae-169">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-169">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="d11ae-170">Backup</span><span class="sxs-lookup"><span data-stu-id="d11ae-170">Backup</span></span>

* <span data-ttu-id="d11ae-171">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-171">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="d11ae-172">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d11ae-172">BatchAI</span></span>

* <span data-ttu-id="d11ae-173">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-173">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="d11ae-174">Cloud</span><span class="sxs-lookup"><span data-stu-id="d11ae-174">Cloud</span></span>

* <span data-ttu-id="d11ae-175">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-175">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-176">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-176">Container</span></span>

* <span data-ttu-id="d11ae-177">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-177">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="d11ae-178">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-178">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="d11ae-179">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-179">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-180">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-180">Extension</span></span>

* <span data-ttu-id="d11ae-181">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-181">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-182">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-182">Network</span></span>

* <span data-ttu-id="d11ae-183">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="d11ae-183">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="d11ae-184">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d11ae-184">Rdbms</span></span>

* <span data-ttu-id="d11ae-185">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-185">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-186">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-186">Resource</span></span>

* <span data-ttu-id="d11ae-187">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-187">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-188">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-188">VM</span></span>

* <span data-ttu-id="d11ae-189">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-189">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="d11ae-190">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-190">June 25, 2018</span></span>

<span data-ttu-id="d11ae-191">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="d11ae-191">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="d11ae-192">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="d11ae-192">CLI</span></span>

* <span data-ttu-id="d11ae-193">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="d11ae-193">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="d11ae-194">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-194">June 19, 2018</span></span>

<span data-ttu-id="d11ae-195">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="d11ae-195">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-196">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-196">Core</span></span>

* <span data-ttu-id="d11ae-197">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-197">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-198">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-198">ACR</span></span>

* <span data-ttu-id="d11ae-199">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-199">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="d11ae-200">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-200">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-201">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-201">ACS</span></span>

* <span data-ttu-id="d11ae-202">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-202">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="d11ae-203">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-203">Added `--update` support</span></span>
* <span data-ttu-id="d11ae-204">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-204">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="d11ae-205">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-205">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="d11ae-206">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-206">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="d11ae-207">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="d11ae-207">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="d11ae-208">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-208">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="d11ae-209">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-209">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-210">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-210">AppService</span></span>

* <span data-ttu-id="d11ae-211">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-211">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="d11ae-212">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-212">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-213">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-213">Batch</span></span>

* <span data-ttu-id="d11ae-214">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-214">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d11ae-215">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d11ae-215">Batch AI</span></span>

* <span data-ttu-id="d11ae-216">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-216">Added support for workspaces.</span></span> <span data-ttu-id="d11ae-217">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="d11ae-217">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="d11ae-218">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-218">Added support for experiments.</span></span> <span data-ttu-id="d11ae-219">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-219">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="d11ae-220">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-220">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="d11ae-221">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-221">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="d11ae-222">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="d11ae-222">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="d11ae-223">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-223">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="d11ae-224">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-224">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="d11ae-225">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-225">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="d11ae-226">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-226">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="d11ae-227">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="d11ae-227">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="d11ae-228">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-228">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="d11ae-229">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="d11ae-229">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="d11ae-230">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-230">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="d11ae-231">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="d11ae-231">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="d11ae-232">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-232">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="d11ae-233">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="d11ae-233">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="d11ae-234">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-234">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="d11ae-235">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-235">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="d11ae-236">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-236">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="d11ae-237">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-237">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="d11ae-238">Karten</span><span class="sxs-lookup"><span data-stu-id="d11ae-238">Maps</span></span>

* <span data-ttu-id="d11ae-239">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-239">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-240">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-240">Network</span></span>

* <span data-ttu-id="d11ae-241">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="d11ae-241">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="d11ae-242">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="d11ae-242">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="d11ae-243">#6502</span><span class="sxs-lookup"><span data-stu-id="d11ae-243">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="d11ae-244">Reservations</span><span class="sxs-lookup"><span data-stu-id="d11ae-244">Reservations</span></span>

* <span data-ttu-id="d11ae-245">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-245">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="d11ae-246">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-246">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="d11ae-247">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-247">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="d11ae-248">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-248">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="d11ae-249">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-249">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="d11ae-250">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-250">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-251">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-251">Role</span></span>

* <span data-ttu-id="d11ae-252">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-252">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-253">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-253">SQL</span></span>

* <span data-ttu-id="d11ae-254">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-254">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-255">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-255">Storage</span></span>

* <span data-ttu-id="d11ae-256">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-256">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-257">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-257">VM</span></span>

* <span data-ttu-id="d11ae-258">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="d11ae-258">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="d11ae-259">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-259">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="d11ae-260">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-260">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d11ae-261">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-261">June 13, 2018</span></span>

<span data-ttu-id="d11ae-262">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="d11ae-262">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-263">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-263">Core</span></span>

* <span data-ttu-id="d11ae-264">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="d11ae-264">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d11ae-265">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-265">June 13, 2018</span></span>

<span data-ttu-id="d11ae-266">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d11ae-266">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d11ae-267">AKS</span><span class="sxs-lookup"><span data-stu-id="d11ae-267">AKS</span></span>

* <span data-ttu-id="d11ae-268">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-268">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d11ae-269">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-269">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="d11ae-270">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-270">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d11ae-271">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-271">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d11ae-272">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-272">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-273">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-273">AppService</span></span>

* <span data-ttu-id="d11ae-274">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-274">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d11ae-275">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-275">June 5, 2018</span></span>

<span data-ttu-id="d11ae-276">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d11ae-276">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-277">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-277">Interactive</span></span>

* <span data-ttu-id="d11ae-278">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-278">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d11ae-279">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-279">June 5, 2018</span></span>

<span data-ttu-id="d11ae-280">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d11ae-280">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-281">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-281">Core</span></span>

* <span data-ttu-id="d11ae-282">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-282">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d11ae-283">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="d11ae-283">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-284">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-284">ACR</span></span>

* <span data-ttu-id="d11ae-285">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-285">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d11ae-286">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-286">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d11ae-287">AKS</span><span class="sxs-lookup"><span data-stu-id="d11ae-287">AKS</span></span>

* <span data-ttu-id="d11ae-288">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-288">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-289">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-289">Batch</span></span>

* <span data-ttu-id="d11ae-290">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d11ae-290">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-291">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-291">IOT</span></span>

* <span data-ttu-id="d11ae-292">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-292">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-293">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-293">Network</span></span>

* <span data-ttu-id="d11ae-294">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-294">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d11ae-295">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="d11ae-295">Policy Insights</span></span>

* <span data-ttu-id="d11ae-296">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-296">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d11ae-297">ARM</span><span class="sxs-lookup"><span data-stu-id="d11ae-297">ARM</span></span>

* <span data-ttu-id="d11ae-298">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-298">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-299">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-299">SQL</span></span>

* <span data-ttu-id="d11ae-300">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-300">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d11ae-301">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-301">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d11ae-302">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-302">Storage</span></span>

* <span data-ttu-id="d11ae-303">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="d11ae-303">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-304">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-304">VM</span></span>

* <span data-ttu-id="d11ae-305">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-305">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d11ae-306">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-306">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d11ae-307">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-307">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d11ae-308">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-308">May 22, 2018</span></span>

<span data-ttu-id="d11ae-309">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d11ae-309">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-310">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-310">Core</span></span>

* <span data-ttu-id="d11ae-311">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-311">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-312">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-312">ACS</span></span>

* <span data-ttu-id="d11ae-313">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-313">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d11ae-314">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-314">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-315">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-315">AppService</span></span>

* <span data-ttu-id="d11ae-316">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="d11ae-316">Improved generic update commands</span></span>
* <span data-ttu-id="d11ae-317">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-317">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-318">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-318">Container</span></span>

* <span data-ttu-id="d11ae-319">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-319">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d11ae-320">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-320">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-321">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-321">Extension</span></span>

* <span data-ttu-id="d11ae-322">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-322">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-323">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-323">Interactive</span></span>

* <span data-ttu-id="d11ae-324">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d11ae-324">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d11ae-325">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="d11ae-325">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-326">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-326">KeyVault</span></span>

* <span data-ttu-id="d11ae-327">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d11ae-327">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-328">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-328">Network</span></span>

* <span data-ttu-id="d11ae-329">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="d11ae-329">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d11ae-330">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="d11ae-330">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-331">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-331">SQL</span></span>

* <span data-ttu-id="d11ae-332">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="d11ae-332">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d11ae-333">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-333">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d11ae-334">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-334">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="d11ae-335">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="d11ae-335">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d11ae-336">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-336">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d11ae-337">`requestedServiceObjectiveName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-337">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d11ae-338">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="d11ae-338">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d11ae-339">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-339">`edition`.</span></span> <span data-ttu-id="d11ae-340">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="d11ae-340">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d11ae-341">`elasticPoolName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-341">`elasticPoolName`.</span></span> <span data-ttu-id="d11ae-342">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="d11ae-342">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d11ae-343">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-343">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d11ae-344">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-344">`edition`.</span></span> <span data-ttu-id="d11ae-345">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-345">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d11ae-346">`dtu`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-346">`dtu`.</span></span> <span data-ttu-id="d11ae-347">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-347">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d11ae-348">`databaseDtuMin`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-348">`databaseDtuMin`.</span></span> <span data-ttu-id="d11ae-349">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-349">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d11ae-350">`databaseDtuMax`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-350">`databaseDtuMax`.</span></span> <span data-ttu-id="d11ae-351">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-351">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d11ae-352">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-352">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d11ae-353">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-353">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-354">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-354">Storage</span></span>

* <span data-ttu-id="d11ae-355">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-355">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d11ae-356">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-356">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-357">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-357">VM</span></span>

* <span data-ttu-id="d11ae-358">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-358">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d11ae-359">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-359">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d11ae-360">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-360">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d11ae-361">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-361">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d11ae-362">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-362">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d11ae-363">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-363">May 7, 2018</span></span>

<span data-ttu-id="d11ae-364">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d11ae-364">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-365">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-365">Core</span></span>

* <span data-ttu-id="d11ae-366">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="d11ae-366">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d11ae-367">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-367">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d11ae-368">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d11ae-368">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d11ae-369">#5591</span><span class="sxs-lookup"><span data-stu-id="d11ae-369">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d11ae-370">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-370">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d11ae-371">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="d11ae-371">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d11ae-372">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="d11ae-372">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d11ae-373">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="d11ae-373">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d11ae-374">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-374">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-375">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-375">ACR</span></span>

* <span data-ttu-id="d11ae-376">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-376">Added ACR Build commands</span></span>
* <span data-ttu-id="d11ae-377">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-377">Improved resource not found error messages</span></span>
* <span data-ttu-id="d11ae-378">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="d11ae-378">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d11ae-379">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-379">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d11ae-380">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-380">Improved repository commands error messages</span></span>
* <span data-ttu-id="d11ae-381">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-381">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-382">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-382">ACS</span></span>

* <span data-ttu-id="d11ae-383">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-383">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d11ae-384">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-384">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d11ae-385">AMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-385">AMS</span></span>

* <span data-ttu-id="d11ae-386">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d11ae-386">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-387">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-387">Appservice</span></span>

* <span data-ttu-id="d11ae-388">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="d11ae-388">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d11ae-389">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-389">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d11ae-390">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-390">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d11ae-391">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-391">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d11ae-392">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d11ae-392">Batch AI</span></span>

* <span data-ttu-id="d11ae-393">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-393">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d11ae-394">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d11ae-394">Cognitive Services</span></span>

* <span data-ttu-id="d11ae-395">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="d11ae-395">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d11ae-396">Nutzung</span><span class="sxs-lookup"><span data-stu-id="d11ae-396">Consumption</span></span>

* <span data-ttu-id="d11ae-397">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-397">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-398">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-398">Container</span></span>

* <span data-ttu-id="d11ae-399">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-399">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d11ae-400">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d11ae-400">Cosmos DB</span></span>

* <span data-ttu-id="d11ae-401">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d11ae-401">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d11ae-402">DMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-402">DMS</span></span>

* <span data-ttu-id="d11ae-403">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-403">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-404">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-404">Extension</span></span>

* <span data-ttu-id="d11ae-405">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-405">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-406">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-406">Interactive</span></span>

* <span data-ttu-id="d11ae-407">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="d11ae-407">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d11ae-408">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="d11ae-408">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d11ae-409">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-409">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d11ae-410">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-410">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d11ae-411">Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-411">Lab</span></span>

* <span data-ttu-id="d11ae-412">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-412">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-413">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-413">Network</span></span>

* <span data-ttu-id="d11ae-414">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="d11ae-414">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d11ae-415">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-415">Profile</span></span>

* <span data-ttu-id="d11ae-416">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-416">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d11ae-417">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-417">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d11ae-418">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-418">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d11ae-419">Redis</span><span class="sxs-lookup"><span data-stu-id="d11ae-419">Redis</span></span>

* <span data-ttu-id="d11ae-420">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-420">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d11ae-421">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-421">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d11ae-422">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-422">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d11ae-423">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-423">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d11ae-424">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-424">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-425">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-425">Role</span></span>

* <span data-ttu-id="d11ae-426">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-426">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-427">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-427">Storage</span></span>

* <span data-ttu-id="d11ae-428">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-428">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d11ae-429">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="d11ae-429">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d11ae-430">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="d11ae-430">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d11ae-431">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="d11ae-431">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d11ae-432">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="d11ae-432">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-433">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-433">VM</span></span>

* <span data-ttu-id="d11ae-434">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-434">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d11ae-435">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-435">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d11ae-436">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="d11ae-436">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d11ae-437">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-437">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d11ae-438">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="d11ae-438">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d11ae-439">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-439">Added write accelerator support</span></span>
* <span data-ttu-id="d11ae-440">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-440">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d11ae-441">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="d11ae-441">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d11ae-442">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="d11ae-442">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d11ae-443">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-443">April 10, 2018</span></span>

<span data-ttu-id="d11ae-444">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d11ae-444">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-445">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-445">ACR</span></span>

* <span data-ttu-id="d11ae-446">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="d11ae-446">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-447">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-447">ACS</span></span>

* <span data-ttu-id="d11ae-448">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-448">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-449">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-449">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d11ae-451">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-451">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d11ae-452">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d11ae-452">BatchAI</span></span>

* <span data-ttu-id="d11ae-453">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-453">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="d11ae-454">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="d11ae-454">Job level mounting</span></span>
 - <span data-ttu-id="d11ae-455">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="d11ae-455">Environment variables with secret values</span></span>
 - <span data-ttu-id="d11ae-456">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="d11ae-456">Performance counters settings</span></span>
 - <span data-ttu-id="d11ae-457">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="d11ae-457">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="d11ae-458">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="d11ae-458">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="d11ae-459">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="d11ae-459">Usage and limits reporting</span></span>
 - <span data-ttu-id="d11ae-460">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="d11ae-460">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="d11ae-461">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="d11ae-461">Support for custom images</span></span>
 - <span data-ttu-id="d11ae-462">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-462">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d11ae-463">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="d11ae-463">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d11ae-464">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-464">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d11ae-465">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="d11ae-465">National clouds are supported</span></span>
* <span data-ttu-id="d11ae-466">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-466">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d11ae-467">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="d11ae-467">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d11ae-468">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-468">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d11ae-469">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="d11ae-469">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d11ae-470">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="d11ae-470">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d11ae-471">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="d11ae-471">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d11ae-472">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="d11ae-472">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d11ae-473">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-473">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d11ae-474">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="d11ae-474">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d11ae-475">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-475">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d11ae-476">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="d11ae-476">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d11ae-477">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-477">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d11ae-478">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="d11ae-478">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d11ae-479">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="d11ae-479">Billing</span></span>

* <span data-ttu-id="d11ae-480">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-480">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d11ae-481">Nutzung</span><span class="sxs-lookup"><span data-stu-id="d11ae-481">Consumption</span></span>

* <span data-ttu-id="d11ae-482">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-482">Added `marketplace` commands</span></span>
* <span data-ttu-id="d11ae-483">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-483">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d11ae-484">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-484">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d11ae-485">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-485">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d11ae-486">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-486">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d11ae-487">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-487">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-488">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-488">Container</span></span>

* <span data-ttu-id="d11ae-489">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-489">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d11ae-490">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-490">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-491">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-491">Extension</span></span>

* <span data-ttu-id="d11ae-492">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-492">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-493">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-493">Interactive</span></span>

* <span data-ttu-id="d11ae-494">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="d11ae-494">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d11ae-495">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-495">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d11ae-496">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-496">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-497">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-497">Network</span></span>

* <span data-ttu-id="d11ae-498">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-498">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d11ae-499">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-499">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d11ae-500">#4910</span><span class="sxs-lookup"><span data-stu-id="d11ae-500">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d11ae-501">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-501">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="d11ae-502">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-502">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d11ae-503">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-503">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d11ae-504">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-504">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d11ae-505">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-505">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-506">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-506">Profile</span></span>

* <span data-ttu-id="d11ae-507">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-507">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d11ae-508">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-508">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d11ae-509">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-509">RDBMS</span></span>

* <span data-ttu-id="d11ae-510">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-510">Added `georestore` command</span></span>
* <span data-ttu-id="d11ae-511">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-511">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-512">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-512">Resource</span></span>

* <span data-ttu-id="d11ae-513">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-513">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d11ae-514">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-514">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-515">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-515">SQL</span></span>

* <span data-ttu-id="d11ae-516">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-516">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-517">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-517">Storage</span></span>

* <span data-ttu-id="d11ae-518">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-518">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-519">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-519">VM</span></span>

* <span data-ttu-id="d11ae-520">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-520">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d11ae-521">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-521">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d11ae-523">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-523">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d11ae-524">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="d11ae-524">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d11ae-525">#5718</span><span class="sxs-lookup"><span data-stu-id="d11ae-525">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d11ae-526">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="d11ae-526">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d11ae-527">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-527">March 27, 2018</span></span>

<span data-ttu-id="d11ae-528">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d11ae-528">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-529">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-529">Core</span></span>

* <span data-ttu-id="d11ae-530">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="d11ae-530">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-531">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-531">ACS</span></span>

* <span data-ttu-id="d11ae-532">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d11ae-532">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-533">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-533">Appservice</span></span>

* <span data-ttu-id="d11ae-534">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-534">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d11ae-535">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-535">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d11ae-536">Backup</span><span class="sxs-lookup"><span data-stu-id="d11ae-536">Backup</span></span>

* <span data-ttu-id="d11ae-537">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-537">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d11ae-538">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="d11ae-538">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d11ae-539">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d11ae-539">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d11ae-540">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="d11ae-540">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-541">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-541">Container</span></span>

* <span data-ttu-id="d11ae-542">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-542">Added `container exec` command.</span></span> <span data-ttu-id="d11ae-543">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="d11ae-543">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d11ae-544">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="d11ae-544">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-545">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-545">Extension</span></span>

* <span data-ttu-id="d11ae-546">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="d11ae-546">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d11ae-547">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="d11ae-547">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d11ae-548">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="d11ae-548">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-549">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-549">Interactive</span></span>

* <span data-ttu-id="d11ae-550">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-550">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d11ae-551">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-551">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d11ae-552">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d11ae-552">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d11ae-553">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="d11ae-553">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d11ae-554">Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-554">Lab</span></span>

* <span data-ttu-id="d11ae-555">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-555">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-556">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-556">Monitor</span></span>

* <span data-ttu-id="d11ae-557">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="d11ae-557">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d11ae-558">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="d11ae-558">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d11ae-559">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="d11ae-559">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-560">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-560">Network</span></span>

* <span data-ttu-id="d11ae-561">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-561">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-562">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-562">Profile</span></span>

* <span data-ttu-id="d11ae-563">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-563">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d11ae-564">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-564">RDBMS</span></span>

* <span data-ttu-id="d11ae-565">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-565">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-566">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-566">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d11ae-568">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-568">Role</span></span>

* <span data-ttu-id="d11ae-569">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-569">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d11ae-570">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="d11ae-570">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d11ae-571">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-571">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d11ae-572">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-572">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d11ae-573">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-573">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-574">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-574">Storage</span></span>

* <span data-ttu-id="d11ae-575">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-575">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d11ae-576">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="d11ae-576">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-577">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-577">VM</span></span>

* <span data-ttu-id="d11ae-578">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-578">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d11ae-579">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-579">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d11ae-580">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="d11ae-580">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d11ae-581">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="d11ae-581">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d11ae-582">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-582">March 13, 2018</span></span>

<span data-ttu-id="d11ae-583">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d11ae-583">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-584">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-584">ACR</span></span>

* <span data-ttu-id="d11ae-585">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-585">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d11ae-586">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-586">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d11ae-587">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-587">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-588">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-588">ACS</span></span>

* <span data-ttu-id="d11ae-589">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-589">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d11ae-590">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-590">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d11ae-591">Advisor</span><span class="sxs-lookup"><span data-stu-id="d11ae-591">Advisor</span></span>

* <span data-ttu-id="d11ae-592">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-592">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d11ae-593">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-593">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d11ae-594">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-594">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="d11ae-595">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-595">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d11ae-596">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-596">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-597">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-597">Appservice</span></span>

* <span data-ttu-id="d11ae-598">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-598">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d11ae-599">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-599">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d11ae-600">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="d11ae-600">Eventhubs</span></span>

* <span data-ttu-id="d11ae-601">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-601">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-602">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-602">Extension</span></span>

* <span data-ttu-id="d11ae-603">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="d11ae-603">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-604">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-604">Interactive</span></span>

* <span data-ttu-id="d11ae-605">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="d11ae-605">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d11ae-606">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="d11ae-606">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d11ae-607">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="d11ae-607">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d11ae-608">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-608">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-609">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-609">Monitor</span></span>

* <span data-ttu-id="d11ae-610">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-610">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d11ae-611">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-611">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d11ae-612">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-612">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d11ae-613">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-613">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-614">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-614">Network</span></span>

* <span data-ttu-id="d11ae-615">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-615">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d11ae-616">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-616">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d11ae-617">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-617">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d11ae-618">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-618">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-619">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-619">Profile</span></span>

* <span data-ttu-id="d11ae-620">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-620">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d11ae-621">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-621">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d11ae-622">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-622">RDBMS</span></span>

* <span data-ttu-id="d11ae-623">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-623">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d11ae-624">Service Bus</span><span class="sxs-lookup"><span data-stu-id="d11ae-624">Service Bus</span></span>

* <span data-ttu-id="d11ae-625">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-625">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-626">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-626">Storage</span></span>

* <span data-ttu-id="d11ae-627">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="d11ae-627">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d11ae-628">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="d11ae-628">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-629">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-629">VM</span></span>

* <span data-ttu-id="d11ae-630">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="d11ae-630">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d11ae-631">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-631">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d11ae-632">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-632">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d11ae-633">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-633">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d11ae-634">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-634">February 27, 2018</span></span>

<span data-ttu-id="d11ae-635">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d11ae-635">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-636">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-636">Core</span></span>

* <span data-ttu-id="d11ae-637">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-637">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d11ae-638">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-638">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d11ae-639">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-639">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-640">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-640">ACS</span></span>

* <span data-ttu-id="d11ae-641">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-641">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d11ae-642">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="d11ae-642">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d11ae-643">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-643">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d11ae-644">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-644">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-645">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-645">Appservice</span></span>

* <span data-ttu-id="d11ae-646">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d11ae-646">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d11ae-647">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="d11ae-647">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d11ae-648">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d11ae-648">Cognitive Services</span></span>

* <span data-ttu-id="d11ae-649">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-649">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d11ae-650">Nutzung</span><span class="sxs-lookup"><span data-stu-id="d11ae-650">Consumption</span></span>

* <span data-ttu-id="d11ae-651">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-651">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d11ae-652">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-652">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-653">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-653">Container</span></span>

* <span data-ttu-id="d11ae-654">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="d11ae-654">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-655">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-655">Network</span></span>

* <span data-ttu-id="d11ae-656">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d11ae-656">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-657">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-657">Resource</span></span>

* <span data-ttu-id="d11ae-658">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="d11ae-658">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-659">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-659">Role</span></span>

* <span data-ttu-id="d11ae-660">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-660">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-661">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-661">SQL</span></span>

* <span data-ttu-id="d11ae-662">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="d11ae-662">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-663">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-663">Storage</span></span>

* <span data-ttu-id="d11ae-664">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-664">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-665">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-665">VM</span></span>

* <span data-ttu-id="d11ae-666">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-666">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d11ae-667">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-667">February 13, 2018</span></span>

<span data-ttu-id="d11ae-668">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d11ae-668">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-669">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-669">Core</span></span>

* <span data-ttu-id="d11ae-670">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-670">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-671">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-671">ACS</span></span>

* <span data-ttu-id="d11ae-672">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-672">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d11ae-673">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-673">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d11ae-674">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-674">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d11ae-675">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-675">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d11ae-676">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-676">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d11ae-677">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-677">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d11ae-678">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="d11ae-678">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d11ae-679">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="d11ae-679">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-680">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-680">Appservice</span></span>

* <span data-ttu-id="d11ae-681">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="d11ae-681">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d11ae-682">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-682">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d11ae-683">CDN</span><span class="sxs-lookup"><span data-stu-id="d11ae-683">CDN</span></span>

* <span data-ttu-id="d11ae-684">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-684">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-685">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-685">Container</span></span>

* <span data-ttu-id="d11ae-686">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-686">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d11ae-687">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-687">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d11ae-688">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d11ae-688">CosmosDB</span></span>

* <span data-ttu-id="d11ae-689">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-689">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-690">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-690">Extension</span></span>

* <span data-ttu-id="d11ae-691">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-691">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d11ae-692">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-692">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d11ae-693">Feedback</span><span class="sxs-lookup"><span data-stu-id="d11ae-693">Feedback</span></span>

* <span data-ttu-id="d11ae-694">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-694">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-695">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-695">Interactive</span></span>

* <span data-ttu-id="d11ae-696">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-696">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d11ae-697">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-697">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-698">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-698">IoT</span></span>

* <span data-ttu-id="d11ae-699">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="d11ae-699">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d11ae-700">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="d11ae-700">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d11ae-701">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-701">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d11ae-702">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-702">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-703">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-703">Monitor</span></span>

* <span data-ttu-id="d11ae-704">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-704">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-705">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-705">Network</span></span>

* <span data-ttu-id="d11ae-706">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="d11ae-706">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d11ae-707">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-707">Profile</span></span>

* <span data-ttu-id="d11ae-708">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="d11ae-708">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-709">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-709">Resource</span></span>

* <span data-ttu-id="d11ae-710">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-710">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-711">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-711">Role</span></span>

* <span data-ttu-id="d11ae-712">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-712">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-713">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-713">SQL</span></span>

* <span data-ttu-id="d11ae-714">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-714">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d11ae-715">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-715">Added `sql db rename`</span></span>
* <span data-ttu-id="d11ae-716">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-716">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-717">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-717">Storage</span></span>

* <span data-ttu-id="d11ae-718">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-718">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-719">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-719">VM</span></span>

* <span data-ttu-id="d11ae-720">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-720">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d11ae-721">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-721">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d11ae-722">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="d11ae-722">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d11ae-723">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-723">January 31, 2018</span></span>

<span data-ttu-id="d11ae-724">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d11ae-724">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-725">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-725">Core</span></span>

* <span data-ttu-id="d11ae-726">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-726">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d11ae-727">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-727">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d11ae-728">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d11ae-728">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d11ae-729">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-729">Use `--verbose` to see</span></span>
* <span data-ttu-id="d11ae-730">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-730">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-731">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-731">ACS</span></span>

* <span data-ttu-id="d11ae-732">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="d11ae-732">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d11ae-733">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-733">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-734">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-734">Appservice</span></span>

* <span data-ttu-id="d11ae-735">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="d11ae-735">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d11ae-736">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-736">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d11ae-737">CDN</span><span class="sxs-lookup"><span data-stu-id="d11ae-737">CDN</span></span>

* <span data-ttu-id="d11ae-738">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-738">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d11ae-739">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d11ae-739">CosmosDB</span></span>

* <span data-ttu-id="d11ae-740">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-740">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-741">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-741">Interactive</span></span>

* <span data-ttu-id="d11ae-742">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-742">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-743">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-743">Network</span></span>

* <span data-ttu-id="d11ae-744">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-744">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d11ae-745">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="d11ae-745">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d11ae-746">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-746">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d11ae-747">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-747">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d11ae-748">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-748">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d11ae-749">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="d11ae-749">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d11ae-750">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-750">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d11ae-751">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-751">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d11ae-752">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-752">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="d11ae-753">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="d11ae-753">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-754">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-754">Profile</span></span>

* <span data-ttu-id="d11ae-755">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-755">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-756">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-756">Resource</span></span>

* <span data-ttu-id="d11ae-757">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="d11ae-757">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-758">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-758">Storage</span></span>

* <span data-ttu-id="d11ae-759">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-759">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d11ae-760">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-760">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d11ae-761">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="d11ae-761">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="d11ae-762">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-762">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d11ae-763">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="d11ae-763">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-764">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-764">VM</span></span>

* <span data-ttu-id="d11ae-765">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-765">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d11ae-766">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="d11ae-766">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d11ae-767">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-767">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d11ae-768">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-768">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d11ae-769">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="d11ae-769">January 17, 2018</span></span>

<span data-ttu-id="d11ae-770">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d11ae-770">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-771">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-771">ACR</span></span>

* <span data-ttu-id="d11ae-772">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-772">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d11ae-773">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="d11ae-773">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-774">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-774">ACS</span></span>

* <span data-ttu-id="d11ae-775">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-775">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d11ae-776">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-776">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-777">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-777">Appservice</span></span>

* <span data-ttu-id="d11ae-778">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="d11ae-778">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d11ae-779">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-779">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d11ae-780">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-780">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d11ae-781">Backup</span><span class="sxs-lookup"><span data-stu-id="d11ae-781">Backup</span></span>

* <span data-ttu-id="d11ae-782">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="d11ae-782">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d11ae-783">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-783">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d11ae-784">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="d11ae-784">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d11ae-785">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="d11ae-785">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d11ae-786">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="d11ae-786">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-787">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-787">Batch</span></span>

* <span data-ttu-id="d11ae-788">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="d11ae-788">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d11ae-789">Cloud</span><span class="sxs-lookup"><span data-stu-id="d11ae-789">Cloud</span></span>

* <span data-ttu-id="d11ae-790">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-790">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d11ae-791">Nutzung</span><span class="sxs-lookup"><span data-stu-id="d11ae-791">Consumption</span></span>

* <span data-ttu-id="d11ae-792">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d11ae-792">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d11ae-793">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d11ae-793">Event Grid</span></span>

* <span data-ttu-id="d11ae-794">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="d11ae-794">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d11ae-795">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="d11ae-795">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d11ae-796">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-796">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d11ae-797">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-797">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d11ae-798">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-798">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d11ae-799">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-799">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d11ae-800">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-800">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d11ae-801">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-801">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-802">Interactive</span><span class="sxs-lookup"><span data-stu-id="d11ae-802">Interactive</span></span>

* <span data-ttu-id="d11ae-803">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d11ae-803">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d11ae-804">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-804">Fixed errors on startup</span></span>
* <span data-ttu-id="d11ae-805">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="d11ae-805">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-806">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-806">IoT</span></span>

* <span data-ttu-id="d11ae-807">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-807">Added support for device provisioning service</span></span>
* <span data-ttu-id="d11ae-808">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-808">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d11ae-809">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="d11ae-809">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-810">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-810">Monitor</span></span>

* <span data-ttu-id="d11ae-811">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-811">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d11ae-812">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d11ae-812">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d11ae-813">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-813">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-814">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-814">Network</span></span>

* <span data-ttu-id="d11ae-815">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="d11ae-815">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d11ae-816">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-816">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-817">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-817">Profile</span></span>

* <span data-ttu-id="d11ae-818">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-818">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-819">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-819">Role</span></span>

* <span data-ttu-id="d11ae-820">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="d11ae-820">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d11ae-821">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d11ae-821">Service Fabric</span></span>

* <span data-ttu-id="d11ae-822">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-822">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d11ae-823">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-823">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-824">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-824">VM</span></span>

* <span data-ttu-id="d11ae-825">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="d11ae-825">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d11ae-826">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-826">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d11ae-827">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="d11ae-827">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d11ae-828">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-828">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d11ae-829">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-829">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d11ae-830">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-830">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d11ae-831">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-831">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d11ae-832">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-832">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d11ae-833">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-833">December 19, 2017</span></span>

<span data-ttu-id="d11ae-834">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d11ae-834">Version 2.0.23</span></span>

* <span data-ttu-id="d11ae-835">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-835">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-836">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-836">Container</span></span>

* <span data-ttu-id="d11ae-837">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-837">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-838">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-838">Network</span></span>

* <span data-ttu-id="d11ae-839">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-839">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d11ae-840">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-840">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-841">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-841">Storage</span></span>

* <span data-ttu-id="d11ae-842">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-842">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-843">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-843">VM</span></span>

* <span data-ttu-id="d11ae-844">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-844">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d11ae-845">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-845">December 5, 2017</span></span>

<span data-ttu-id="d11ae-846">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d11ae-846">Version 2.0.22</span></span>

* <span data-ttu-id="d11ae-847">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-847">Removed `az component` commands.</span></span> <span data-ttu-id="d11ae-848">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-848">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-849">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-849">Core</span></span>
* <span data-ttu-id="d11ae-850">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-850">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d11ae-851">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-851">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-852">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-852">ACS</span></span>

* <span data-ttu-id="d11ae-853">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-853">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d11ae-854">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="d11ae-854">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d11ae-855">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="d11ae-855">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d11ae-856">Advisor</span><span class="sxs-lookup"><span data-stu-id="d11ae-856">Advisor</span></span>

* <span data-ttu-id="d11ae-857">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-857">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-858">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-858">Appservice</span></span>

* <span data-ttu-id="d11ae-859">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d11ae-859">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d11ae-860">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="d11ae-860">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d11ae-861">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-861">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d11ae-862">Nutzung</span><span class="sxs-lookup"><span data-stu-id="d11ae-862">Consumption</span></span>

* <span data-ttu-id="d11ae-863">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-863">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-864">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-864">Container</span></span>

* <span data-ttu-id="d11ae-865">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="d11ae-865">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-866">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-866">Monitor</span></span>

* <span data-ttu-id="d11ae-867">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-867">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-868">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-868">Resource</span></span>

* <span data-ttu-id="d11ae-869">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-869">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-870">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-870">Role</span></span>

* <span data-ttu-id="d11ae-871">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-871">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d11ae-872">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-872">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d11ae-873">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d11ae-873">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-874">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-874">SQL</span></span>

* <span data-ttu-id="d11ae-875">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-875">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d11ae-876">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-876">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-877">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-877">VM</span></span>

* <span data-ttu-id="d11ae-878">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-878">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d11ae-879">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-879">November 14, 2017</span></span>

<span data-ttu-id="d11ae-880">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d11ae-880">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-881">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-881">ACR</span></span>

* <span data-ttu-id="d11ae-882">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-882">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d11ae-883">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-883">ACS</span></span>

* <span data-ttu-id="d11ae-884">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-884">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d11ae-885">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="d11ae-885">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d11ae-886">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="d11ae-886">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d11ae-887">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-887">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d11ae-888">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-888">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-889">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-889">Appservice</span></span>

* <span data-ttu-id="d11ae-890">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-890">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d11ae-891">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-891">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d11ae-892">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-892">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d11ae-893">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-893">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d11ae-894">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-894">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d11ae-895">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="d11ae-895">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-896">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-896">Batch</span></span>

* <span data-ttu-id="d11ae-897">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-897">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d11ae-898">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d11ae-898">Batchai</span></span>

* <span data-ttu-id="d11ae-899">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-899">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d11ae-900">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-900">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d11ae-901">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-901">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d11ae-902">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-902">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d11ae-903">Cloud</span><span class="sxs-lookup"><span data-stu-id="d11ae-903">Cloud</span></span>

* <span data-ttu-id="d11ae-904">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="d11ae-904">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-905">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-905">Container</span></span>

* <span data-ttu-id="d11ae-906">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-906">Added support to open multiple ports</span></span>
* <span data-ttu-id="d11ae-907">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-907">Added container group restart policy</span></span>
* <span data-ttu-id="d11ae-908">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-908">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d11ae-909">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-909">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d11ae-910">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d11ae-910">Data Lake Analytics</span></span>

* <span data-ttu-id="d11ae-911">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="d11ae-911">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d11ae-912">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d11ae-912">Data Lake Store</span></span>

* <span data-ttu-id="d11ae-913">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="d11ae-913">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-914">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-914">Extension</span></span>

* <span data-ttu-id="d11ae-915">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-915">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d11ae-916">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d11ae-916">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-917">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-917">IoT</span></span>

* <span data-ttu-id="d11ae-918">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-918">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-919">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-919">Monitor</span></span>

* <span data-ttu-id="d11ae-920">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-920">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-921">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-921">Network</span></span>

* <span data-ttu-id="d11ae-922">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-922">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d11ae-923">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="d11ae-923">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d11ae-924">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="d11ae-924">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d11ae-925">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-925">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d11ae-926">Reservations</span><span class="sxs-lookup"><span data-stu-id="d11ae-926">Reservations</span></span>

* <span data-ttu-id="d11ae-927">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="d11ae-927">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-928">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-928">Resource</span></span>

* <span data-ttu-id="d11ae-929">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-929">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-930">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-930">SQL</span></span>

* <span data-ttu-id="d11ae-931">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-931">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-932">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-932">Storage</span></span>

* <span data-ttu-id="d11ae-933">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-933">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d11ae-934">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="d11ae-934">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d11ae-935">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="d11ae-935">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d11ae-936">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-936">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d11ae-937">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-937">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d11ae-938">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-938">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d11ae-939">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-939">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-940">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-940">VM</span></span>

* <span data-ttu-id="d11ae-941">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="d11ae-941">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d11ae-942">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-942">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d11ae-943">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="d11ae-943">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d11ae-944">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-944">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d11ae-945">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-945">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d11ae-946">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-946">October 24, 2017</span></span>

<span data-ttu-id="d11ae-947">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d11ae-947">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-948">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-948">Core</span></span>

* <span data-ttu-id="d11ae-949">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="d11ae-949">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-950">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-950">ACR</span></span>

* <span data-ttu-id="d11ae-951">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-951">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d11ae-952">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-952">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d11ae-953">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-953">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-954">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-954">ACS</span></span>

* <span data-ttu-id="d11ae-955">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-955">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d11ae-956">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-956">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-957">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-957">Appservice</span></span>

* <span data-ttu-id="d11ae-958">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="d11ae-958">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d11ae-959">Komponente</span><span class="sxs-lookup"><span data-stu-id="d11ae-959">Component</span></span>

* <span data-ttu-id="d11ae-960">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-960">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-961">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-961">Monitor</span></span>

* <span data-ttu-id="d11ae-962">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-962">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-963">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-963">Resource</span></span>

* <span data-ttu-id="d11ae-964">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-964">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d11ae-965">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="d11ae-965">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-966">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-966">VM</span></span>

* <span data-ttu-id="d11ae-967">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-967">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d11ae-968">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-968">October 9, 2017</span></span>

<span data-ttu-id="d11ae-969">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d11ae-969">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-970">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-970">Core</span></span>

* <span data-ttu-id="d11ae-971">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-971">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-972">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-972">Appservice</span></span>

* <span data-ttu-id="d11ae-973">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-973">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-974">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-974">Batch</span></span>

* <span data-ttu-id="d11ae-975">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d11ae-975">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d11ae-976">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-976">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d11ae-977">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-977">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d11ae-978">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-978">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d11ae-979">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d11ae-979">Batchai</span></span>

* <span data-ttu-id="d11ae-980">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-980">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-981">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-981">Keyvault</span></span>

* <span data-ttu-id="d11ae-982">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="d11ae-982">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d11ae-983">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d11ae-983">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d11ae-984">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-984">Network</span></span>

* <span data-ttu-id="d11ae-985">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="d11ae-985">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d11ae-986">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-986">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-987">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-987">Resource</span></span>

* <span data-ttu-id="d11ae-988">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-988">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d11ae-989">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-989">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d11ae-990">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-990">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d11ae-991">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-991">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-992">Sql</span><span class="sxs-lookup"><span data-stu-id="d11ae-992">Sql</span></span>

* <span data-ttu-id="d11ae-993">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-993">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d11ae-994">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-994">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d11ae-995">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-995">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-996">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-996">Storage</span></span>

* <span data-ttu-id="d11ae-997">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-997">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-998">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-998">Vm</span></span>

* <span data-ttu-id="d11ae-999">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="d11ae-999">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d11ae-1000">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1000">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d11ae-1001">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1001">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d11ae-1002">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1002">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d11ae-1003">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1003">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d11ae-1004">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1004">September 22, 2017</span></span>

<span data-ttu-id="d11ae-1005">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="d11ae-1005">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-1006">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-1006">Resource</span></span>

* <span data-ttu-id="d11ae-1007">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1007">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d11ae-1008">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1008">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d11ae-1009">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1009">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d11ae-1010">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1010">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1011">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1011">Network</span></span>

* <span data-ttu-id="d11ae-1012">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1012">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d11ae-1013">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1013">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d11ae-1014">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1014">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d11ae-1015">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1015">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d11ae-1016">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1016">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d11ae-1017">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1017">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d11ae-1018">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1018">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1019">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1019">Storage</span></span>

* <span data-ttu-id="d11ae-1020">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1020">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d11ae-1021">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="d11ae-1021">Eventgrid</span></span>

* <span data-ttu-id="d11ae-1022">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1022">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-1023">SQL</span></span>

* <span data-ttu-id="d11ae-1024">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1024">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d11ae-1025">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1025">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d11ae-1026">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1026">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-1027">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-1027">Keyvault</span></span>

* <span data-ttu-id="d11ae-1028">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1028">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1029">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1029">VM</span></span>

* <span data-ttu-id="d11ae-1030">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1030">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d11ae-1031">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1031">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d11ae-1032">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1032">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d11ae-1033">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1033">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d11ae-1034">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1034">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d11ae-1035">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1035">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1036">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1036">ACS</span></span>

* <span data-ttu-id="d11ae-1037">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1037">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1038">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1038">Appservice</span></span>

* <span data-ttu-id="d11ae-1039">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1039">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d11ae-1040">Backup</span><span class="sxs-lookup"><span data-stu-id="d11ae-1040">Backup</span></span>

* <span data-ttu-id="d11ae-1041">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="d11ae-1041">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d11ae-1042">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1042">September 11, 2017</span></span>

<span data-ttu-id="d11ae-1043">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d11ae-1043">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d11ae-1044">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-1044">Core</span></span>

* <span data-ttu-id="d11ae-1045">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1045">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d11ae-1046">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="d11ae-1046">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1047">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1047">Acs</span></span>

* <span data-ttu-id="d11ae-1048">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1048">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d11ae-1049">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1049">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1050">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1050">Appservice</span></span>

* <span data-ttu-id="d11ae-1051">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="d11ae-1051">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d11ae-1052">CDN</span><span class="sxs-lookup"><span data-stu-id="d11ae-1052">CDN</span></span>

* <span data-ttu-id="d11ae-1053">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1053">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d11ae-1054">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d11ae-1054">Extension</span></span>

* <span data-ttu-id="d11ae-1055">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-1055">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-1056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-1056">Keyvault</span></span>

* <span data-ttu-id="d11ae-1057">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="d11ae-1057">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1058">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1058">Network</span></span>

* <span data-ttu-id="d11ae-1059">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1059">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d11ae-1060">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1060">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d11ae-1061">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1061">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d11ae-1062">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1062">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d11ae-1063">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1063">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-1064">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-1064">Resource</span></span>

* <span data-ttu-id="d11ae-1065">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1065">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d11ae-1066">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1066">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d11ae-1067">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1067">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d11ae-1068">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-1068">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-1069">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-1069">SQL</span></span>

* <span data-ttu-id="d11ae-1070">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1070">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1071">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1071">VM</span></span>

* <span data-ttu-id="d11ae-1072">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-1072">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d11ae-1073">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1073">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d11ae-1074">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1074">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d11ae-1075">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1075">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d11ae-1076">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1076">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d11ae-1077">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1077">August 31, 2017</span></span>

<span data-ttu-id="d11ae-1078">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d11ae-1078">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-1079">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-1079">Keyvault</span></span>

* <span data-ttu-id="d11ae-1080">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1080">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d11ae-1081">Sf</span><span class="sxs-lookup"><span data-stu-id="d11ae-1081">Sf</span></span>

* <span data-ttu-id="d11ae-1082">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1082">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1083">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1083">Storage</span></span>

* <span data-ttu-id="d11ae-1084">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1084">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d11ae-1085">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="d11ae-1085">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d11ae-1086">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1086">August 28, 2017</span></span>

<span data-ttu-id="d11ae-1087">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d11ae-1087">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d11ae-1088">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1088">CLI</span></span>

* <span data-ttu-id="d11ae-1089">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1089">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1090">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1090">ACS</span></span>

* <span data-ttu-id="d11ae-1091">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1091">Corrected preview regions</span></span>
* <span data-ttu-id="d11ae-1092">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1092">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d11ae-1093">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1093">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1094">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1094">Appservice</span></span>

* <span data-ttu-id="d11ae-1095">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1095">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d11ae-1096">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1096">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d11ae-1097">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1097">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d11ae-1098">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1098">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d11ae-1099">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1099">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-1100">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-1100">IoT</span></span>

* <span data-ttu-id="d11ae-1101">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="d11ae-1101">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1102">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1102">Network</span></span>

* <span data-ttu-id="d11ae-1103">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1103">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d11ae-1104">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1104">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d11ae-1105">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1105">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d11ae-1106">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1106">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d11ae-1107">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1107">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-1108">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-1108">Profile</span></span>

* <span data-ttu-id="d11ae-1109">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1109">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d11ae-1110">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d11ae-1110">Service Fabric</span></span>

* <span data-ttu-id="d11ae-1111">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="d11ae-1111">Preview release</span></span>
* <span data-ttu-id="d11ae-1112">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1112">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d11ae-1113">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1113">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d11ae-1114">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1114">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1115">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1115">Storage</span></span>

* <span data-ttu-id="d11ae-1116">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1116">Enabled setting blob tier</span></span>
* <span data-ttu-id="d11ae-1117">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1117">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d11ae-1118">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1118">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d11ae-1119">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1119">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d11ae-1120">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1120">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d11ae-1121">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1121">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1122">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1122">VM</span></span>

* <span data-ttu-id="d11ae-1123">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1123">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d11ae-1124">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1124">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d11ae-1125">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1125">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d11ae-1126">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1126">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d11ae-1127">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1127">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d11ae-1128">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1128">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d11ae-1129">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1129">August 15, 2017</span></span>

<span data-ttu-id="d11ae-1130">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d11ae-1130">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1131">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1131">ACS</span></span>

* <span data-ttu-id="d11ae-1132">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1132">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1133">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1133">Appservice</span></span>

* <span data-ttu-id="d11ae-1134">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1134">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d11ae-1135">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d11ae-1135">Event Grid</span></span>

* <span data-ttu-id="d11ae-1136">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1136">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d11ae-1137">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1137">August 11, 2017</span></span>

<span data-ttu-id="d11ae-1138">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d11ae-1138">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1139">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1139">ACS</span></span>

* <span data-ttu-id="d11ae-1140">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1140">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-1141">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-1141">Batch</span></span>

* <span data-ttu-id="d11ae-1142">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1142">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d11ae-1143">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1143">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d11ae-1144">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1144">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d11ae-1145">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1145">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d11ae-1146">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="d11ae-1146">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d11ae-1147">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1147">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d11ae-1148">Komponente</span><span class="sxs-lookup"><span data-stu-id="d11ae-1148">Component</span></span>

* <span data-ttu-id="d11ae-1149">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1149">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d11ae-1150">Container</span><span class="sxs-lookup"><span data-stu-id="d11ae-1150">Container</span></span>

* <span data-ttu-id="d11ae-1151">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="d11ae-1151">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d11ae-1152">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d11ae-1152">Data Lake Store</span></span>

* <span data-ttu-id="d11ae-1153">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1153">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d11ae-1154">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d11ae-1154">Event Grid</span></span>

* <span data-ttu-id="d11ae-1155">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d11ae-1155">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1156">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1156">Network</span></span>

* <span data-ttu-id="d11ae-1157">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1157">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d11ae-1158">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-1158">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d11ae-1159">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1159">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d11ae-1160">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1160">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-1161">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-1161">Profile</span></span>

* <span data-ttu-id="d11ae-1162">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="d11ae-1162">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1163">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1163">Storage</span></span>

* <span data-ttu-id="d11ae-1164">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1164">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1165">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1165">VM</span></span>

* <span data-ttu-id="d11ae-1166">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1166">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d11ae-1167">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1167">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d11ae-1168">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1168">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d11ae-1169">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="d11ae-1169">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d11ae-1170">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1170">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d11ae-1171">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1171">July 28, 2017</span></span>

<span data-ttu-id="d11ae-1172">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d11ae-1172">Version 2.0.12</span></span>

* <span data-ttu-id="d11ae-1173">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1173">Added container commands</span></span>
* <span data-ttu-id="d11ae-1174">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1174">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d11ae-1175">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-1175">Core</span></span>

* <span data-ttu-id="d11ae-1176">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1176">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d11ae-1177">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1177">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d11ae-1178">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="d11ae-1178">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d11ae-1179">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1179">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d11ae-1180">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1180">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d11ae-1181">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1181">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d11ae-1182">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1182">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d11ae-1183">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1183">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d11ae-1184">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1184">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d11ae-1185">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-1185">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d11ae-1186">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="d11ae-1186">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d11ae-1187">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1187">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d11ae-1188">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1188">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d11ae-1189">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1189">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d11ae-1190">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d11ae-1190">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d11ae-1191">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1191">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d11ae-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-1192">ACR</span></span>

* <span data-ttu-id="d11ae-1193">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1193">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d11ae-1194">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1194">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d11ae-1195">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1195">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d11ae-1196">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1196">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d11ae-1197">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1197">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d11ae-1198">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1198">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1199">ACS</span></span>

* <span data-ttu-id="d11ae-1200">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="d11ae-1200">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1201">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1201">Appservice</span></span>

* <span data-ttu-id="d11ae-1202">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="d11ae-1202">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d11ae-1203">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="d11ae-1203">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d11ae-1204">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1204">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d11ae-1205">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1205">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d11ae-1206">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1206">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d11ae-1207">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1207">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d11ae-1208">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1208">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d11ae-1209">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1209">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d11ae-1210">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1210">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d11ae-1211">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1211">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d11ae-1212">Batch</span><span class="sxs-lookup"><span data-stu-id="d11ae-1212">Batch</span></span>

* <span data-ttu-id="d11ae-1213">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1213">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d11ae-1214">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1214">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d11ae-1215">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1215">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d11ae-1216">CDN</span><span class="sxs-lookup"><span data-stu-id="d11ae-1216">CDN</span></span>

* <span data-ttu-id="d11ae-1217">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-1217">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d11ae-1218">Cloud</span><span class="sxs-lookup"><span data-stu-id="d11ae-1218">Cloud</span></span>

* <span data-ttu-id="d11ae-1219">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1219">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d11ae-1220">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="d11ae-1220">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d11ae-1221">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1221">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d11ae-1222">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="d11ae-1222">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d11ae-1223">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1223">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d11ae-1224">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d11ae-1224">CosmosDB</span></span>

* <span data-ttu-id="d11ae-1225">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1225">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d11ae-1226">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1226">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d11ae-1227">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d11ae-1227">Data Lake Analytics</span></span>

* <span data-ttu-id="d11ae-1228">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1228">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d11ae-1229">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1229">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d11ae-1230">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1230">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d11ae-1231">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d11ae-1231">Data Lake Store</span></span>

* <span data-ttu-id="d11ae-1232">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1232">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d11ae-1233">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="d11ae-1233">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d11ae-1234">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1234">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d11ae-1235">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1235">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d11ae-1236">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="d11ae-1236">Interactive</span></span>

* <span data-ttu-id="d11ae-1237">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1237">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d11ae-1238">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1238">Increased test coverage</span></span>
* <span data-ttu-id="d11ae-1239">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-1239">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d11ae-1240">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1240">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d11ae-1241">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1241">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d11ae-1242">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1242">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d11ae-1243">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1243">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d11ae-1244">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1244">Added `--progress` flag</span></span>
* <span data-ttu-id="d11ae-1245">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1245">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d11ae-1246">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1246">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d11ae-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="d11ae-1247">IoT</span></span>

* <span data-ttu-id="d11ae-1248">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="d11ae-1248">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d11ae-1249">(3934)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1249">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d11ae-1250">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="d11ae-1250">Key vault</span></span>

* <span data-ttu-id="d11ae-1251">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1251">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d11ae-1252">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1252">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d11ae-1253">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1253">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d11ae-1254">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1254">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d11ae-1255">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1255">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d11ae-1256">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1256">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d11ae-1257">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1257">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d11ae-1258">(3307)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1258">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d11ae-1259">Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-1259">Lab</span></span>

* <span data-ttu-id="d11ae-1260">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1260">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d11ae-1261">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1261">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-1262">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1262">Monitor</span></span>

* <span data-ttu-id="d11ae-1263">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1263">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d11ae-1264">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1264">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d11ae-1265">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1265">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d11ae-1266">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1266">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d11ae-1267">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1267">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d11ae-1268">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1268">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d11ae-1269">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1269">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d11ae-1270">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1270">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d11ae-1271">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="d11ae-1271">`location` no longer required</span></span>
  * <span data-ttu-id="d11ae-1272">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="d11ae-1272">Add name and ID support for target</span></span>
  * <span data-ttu-id="d11ae-1273">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1273">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d11ae-1274">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1274">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d11ae-1275">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1275">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d11ae-1276">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="d11ae-1276">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d11ae-1277">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1277">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d11ae-1278">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1278">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1279">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1279">Network</span></span>

* <span data-ttu-id="d11ae-1280">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1280">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d11ae-1281">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1281">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d11ae-1282">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1282">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d11ae-1283">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1283">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d11ae-1284">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-1284">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d11ae-1285">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1285">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d11ae-1286">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1286">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d11ae-1287">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1287">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d11ae-1288">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1288">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d11ae-1289">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1289">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d11ae-1290">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1290">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d11ae-1291">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1291">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d11ae-1292">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1292">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d11ae-1293">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1293">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d11ae-1294">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1294">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d11ae-1295">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1295">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d11ae-1296">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1296">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d11ae-1297">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-1297">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d11ae-1298">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1298">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d11ae-1299">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1299">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d11ae-1300">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1300">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d11ae-1301">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1301">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d11ae-1302">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1302">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d11ae-1303">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1303">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d11ae-1304">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1304">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d11ae-1305">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1305">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d11ae-1306">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1306">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-1307">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-1307">Profile</span></span>

* <span data-ttu-id="d11ae-1308">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="d11ae-1308">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d11ae-1309">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="d11ae-1309">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d11ae-1310">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1310">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d11ae-1311">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1311">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d11ae-1312">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="d11ae-1312">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d11ae-1313">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1313">RDBMS</span></span>

* <span data-ttu-id="d11ae-1314">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1314">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d11ae-1315">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1315">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d11ae-1316">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1316">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d11ae-1317">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1317">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-1318">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-1318">Resource</span></span>

* <span data-ttu-id="d11ae-1319">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1319">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d11ae-1320">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="d11ae-1320">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d11ae-1321">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1321">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d11ae-1322">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1322">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d11ae-1323">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1323">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d11ae-1324">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1324">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d11ae-1325">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1325">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d11ae-1326">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1326">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-1327">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-1327">Role</span></span>

* <span data-ttu-id="d11ae-1328">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1328">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d11ae-1329">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1329">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d11ae-1330">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="d11ae-1330">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d11ae-1331">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1331">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d11ae-1332">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1332">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d11ae-1333">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d11ae-1333">Service Fabric</span></span>
* <span data-ttu-id="d11ae-1334">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1334">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d11ae-1335">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1335">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d11ae-1336">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1336">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-1337">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-1337">SQL</span></span>

* <span data-ttu-id="d11ae-1338">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1338">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d11ae-1339">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1339">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d11ae-1340">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1340">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1341">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1341">Storage</span></span>

* <span data-ttu-id="d11ae-1342">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1342">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d11ae-1343">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1343">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d11ae-1344">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1344">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d11ae-1345">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1345">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d11ae-1346">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1346">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d11ae-1347">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1347">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1348">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1348">VM</span></span>

* <span data-ttu-id="d11ae-1349">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d11ae-1349">Support configuring nsg</span></span>
* <span data-ttu-id="d11ae-1350">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-1350">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d11ae-1351">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1351">Support managed service identities</span></span>
* <span data-ttu-id="d11ae-1352">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1352">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d11ae-1353">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1353">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d11ae-1354">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1354">May 10, 2017</span></span>

<span data-ttu-id="d11ae-1355">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d11ae-1355">Version 2.0.6</span></span>

* <span data-ttu-id="d11ae-1356">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1356">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d11ae-1357">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1357">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d11ae-1358">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="d11ae-1358">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d11ae-1359">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1359">Include Cognitive Services module</span></span>
* <span data-ttu-id="d11ae-1360">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1360">Include Service Fabric module</span></span>
* <span data-ttu-id="d11ae-1361">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1361">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d11ae-1362">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="d11ae-1362">Add support for CDN commands</span></span>
* <span data-ttu-id="d11ae-1363">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1363">Remove Container module</span></span>
* <span data-ttu-id="d11ae-1364">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1364">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d11ae-1365">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1365">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d11ae-1366">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-1366">Core</span></span>

* <span data-ttu-id="d11ae-1367">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1367">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d11ae-1368">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1368">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d11ae-1369">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1369">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d11ae-1370">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1370">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d11ae-1371">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1371">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d11ae-1372">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1372">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d11ae-1373">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1373">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d11ae-1374">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1374">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d11ae-1375">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1375">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d11ae-1376">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1376">core: Improved performance</span></span>
* <span data-ttu-id="d11ae-1377">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1377">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d11ae-1378">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-1378">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1379">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1379">ACS</span></span>

* <span data-ttu-id="d11ae-1380">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d11ae-1380">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d11ae-1381">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1381">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d11ae-1382">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1382">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d11ae-1383">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1383">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1384">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1384">AppService</span></span>

* <span data-ttu-id="d11ae-1385">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1385">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d11ae-1386">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1386">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d11ae-1387">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1387">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d11ae-1388">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="d11ae-1388">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d11ae-1389">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1389">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d11ae-1390">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1390">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d11ae-1391">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="d11ae-1391">support slot swap with preview</span></span>
* <span data-ttu-id="d11ae-1392">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1392">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d11ae-1393">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1393">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d11ae-1394">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d11ae-1394">CosmosDB</span></span>

* <span data-ttu-id="d11ae-1395">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d11ae-1395">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d11ae-1396">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1396">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d11ae-1397">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1397">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d11ae-1398">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="d11ae-1398">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d11ae-1399">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d11ae-1399">Data Lake Analytics</span></span>

* <span data-ttu-id="d11ae-1400">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="d11ae-1400">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d11ae-1401">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1401">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d11ae-1402">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1402">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d11ae-1403">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="d11ae-1403">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d11ae-1404">Table</span><span class="sxs-lookup"><span data-stu-id="d11ae-1404">Table</span></span>
  * <span data-ttu-id="d11ae-1405">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="d11ae-1405">Table valued function</span></span>
  * <span data-ttu-id="d11ae-1406">Sicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1406">View</span></span>
  * <span data-ttu-id="d11ae-1407">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1407">Table Statistics.</span></span> <span data-ttu-id="d11ae-1408">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1408">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d11ae-1409">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d11ae-1409">Data Lake Store</span></span>

* <span data-ttu-id="d11ae-1410">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-1410">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d11ae-1411">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1411">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d11ae-1412">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="d11ae-1412">missed help for access show.</span></span> <span data-ttu-id="d11ae-1413">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d11ae-1413">adding it.</span></span> <span data-ttu-id="d11ae-1414">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1414">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d11ae-1415">Suchen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1415">Find</span></span>

* <span data-ttu-id="d11ae-1416">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="d11ae-1416">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d11ae-1417">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d11ae-1417">KeyVault</span></span>

* <span data-ttu-id="d11ae-1418">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1418">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d11ae-1419">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1419">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d11ae-1420">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="d11ae-1420">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d11ae-1421">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="d11ae-1421">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d11ae-1422">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1422">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d11ae-1423">Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-1423">Lab</span></span>

* <span data-ttu-id="d11ae-1424">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="d11ae-1424">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d11ae-1425">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-1425">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d11ae-1426">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="d11ae-1426">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d11ae-1427">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="d11ae-1427">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d11ae-1428">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="d11ae-1428">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d11ae-1429">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1429">Monitor</span></span>

* <span data-ttu-id="d11ae-1430">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1430">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d11ae-1431">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1431">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d11ae-1432">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1432">Network</span></span>

* <span data-ttu-id="d11ae-1433">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1433">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d11ae-1434">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1434">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d11ae-1435">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="d11ae-1435">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d11ae-1436">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1436">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d11ae-1437">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="d11ae-1437">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d11ae-1438">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="d11ae-1438">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d11ae-1439">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1439">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d11ae-1440">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1440">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d11ae-1441">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1441">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d11ae-1442">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="d11ae-1442">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d11ae-1443">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1443">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d11ae-1444">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1444">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d11ae-1445">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="d11ae-1445">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d11ae-1446">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="d11ae-1446">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d11ae-1447">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="d11ae-1447">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d11ae-1448">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1448">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d11ae-1449">Profil</span><span class="sxs-lookup"><span data-stu-id="d11ae-1449">Profile</span></span>

* <span data-ttu-id="d11ae-1450">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1450">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d11ae-1451">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1451">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d11ae-1452">Redis</span><span class="sxs-lookup"><span data-stu-id="d11ae-1452">Redis</span></span>

* <span data-ttu-id="d11ae-1453">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-1453">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d11ae-1454">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1454">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d11ae-1455">Ressource</span><span class="sxs-lookup"><span data-stu-id="d11ae-1455">Resource</span></span>

* <span data-ttu-id="d11ae-1456">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1456">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d11ae-1457">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1457">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d11ae-1458">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1458">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d11ae-1459">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="d11ae-1459">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d11ae-1460">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1460">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d11ae-1461">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1461">Add docs for az lock update.</span></span> <span data-ttu-id="d11ae-1462">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1462">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d11ae-1463">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1463">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d11ae-1464">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1464">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d11ae-1465">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="d11ae-1465">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d11ae-1466">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1466">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d11ae-1467">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1467">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d11ae-1468">Rolle</span><span class="sxs-lookup"><span data-stu-id="d11ae-1468">Role</span></span>

* <span data-ttu-id="d11ae-1469">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1469">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d11ae-1470">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1470">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d11ae-1471">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1471">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d11ae-1472">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="d11ae-1472">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d11ae-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="d11ae-1473">SQL</span></span>

* <span data-ttu-id="d11ae-1474">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1474">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d11ae-1475">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1475">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d11ae-1476">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1476">Storage</span></span>

* <span data-ttu-id="d11ae-1477">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1477">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d11ae-1478">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="d11ae-1478">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d11ae-1479">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="d11ae-1479">Add support for large block blob upload</span></span>
* <span data-ttu-id="d11ae-1480">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="d11ae-1480">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1481">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1481">VM</span></span>

* <span data-ttu-id="d11ae-1482">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="d11ae-1482">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d11ae-1483">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1483">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d11ae-1484">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d11ae-1484">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d11ae-1485">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1485">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d11ae-1486">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1486">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d11ae-1487">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="d11ae-1487">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d11ae-1488">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1488">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d11ae-1489">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1489">April 3, 2017</span></span>

<span data-ttu-id="d11ae-1490">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d11ae-1490">Version 2.0.2</span></span>

<span data-ttu-id="d11ae-1491">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1491">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d11ae-1492">Core</span><span class="sxs-lookup"><span data-stu-id="d11ae-1492">Core</span></span>

* <span data-ttu-id="d11ae-1493">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="d11ae-1493">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d11ae-1494">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1494">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d11ae-1495">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1495">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d11ae-1496">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1496">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d11ae-1497">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1497">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d11ae-1498">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="d11ae-1498">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d11ae-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d11ae-1500">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1500">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d11ae-1501">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="d11ae-1501">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d11ae-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="d11ae-1502">ACS</span></span>

* <span data-ttu-id="d11ae-1503">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1503">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d11ae-1504">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="d11ae-1504">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d11ae-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d11ae-1506">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="d11ae-1506">Add support for windows clusters.</span></span> <span data-ttu-id="d11ae-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d11ae-1508">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="d11ae-1508">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d11ae-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d11ae-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="d11ae-1510">AppService</span></span>

* <span data-ttu-id="d11ae-1511">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1511">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d11ae-1512">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1512">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d11ae-1513">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1513">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d11ae-1514">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1514">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d11ae-1515">DataLake</span><span class="sxs-lookup"><span data-stu-id="d11ae-1515">DataLake</span></span>

* <span data-ttu-id="d11ae-1516">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1516">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d11ae-1517">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="d11ae-1517">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d11ae-1518">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d11ae-1518">DocuemntDB</span></span>

* <span data-ttu-id="d11ae-1519">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1519">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d11ae-1520">VM</span><span class="sxs-lookup"><span data-stu-id="d11ae-1520">VM</span></span>

* <span data-ttu-id="d11ae-1521">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1521">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d11ae-1522">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1522">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d11ae-1523">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1523">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d11ae-1524">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1524">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d11ae-1525">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1525">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d11ae-1526">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1526">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="d11ae-1527">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d11ae-1527">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d11ae-1528">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="d11ae-1528">February 27, 2017</span></span>

<span data-ttu-id="d11ae-1529">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d11ae-1529">Version 2.0.0</span></span>

<span data-ttu-id="d11ae-1530">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1530">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d11ae-1531">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1531">Container Service (acs)</span></span>
- <span data-ttu-id="d11ae-1532">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1532">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d11ae-1533">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d11ae-1533">Networking</span></span>
- <span data-ttu-id="d11ae-1534">Speicher</span><span class="sxs-lookup"><span data-stu-id="d11ae-1534">Storage</span></span>

<span data-ttu-id="d11ae-1535">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1535">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d11ae-1536">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1536">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d11ae-1537">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1537">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d11ae-1538">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="d11ae-1538">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d11ae-1539">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="d11ae-1539">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d11ae-1540">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="d11ae-1540">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d11ae-1541">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1541">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d11ae-1542">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d11ae-1542">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d11ae-1543">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d11ae-1543">Provide feedback from the command line with the `az feedback` command</span></span>

